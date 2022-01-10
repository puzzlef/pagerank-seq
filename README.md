Single-threaded CPU-based PageRank (PR) algorithm ([pull], [CSR]).

All outputs are saved in [out](out/) and a small part of the output is listed
here. Some [charts] are also included below, generated from [sheets]. The input
data used for this experiment is available at the [SuiteSparse Matrix
Collection].

```bash
$ g++ -std=c++17 -O3 main.cxx
$ ./a.out ~/data/web-Stanford.mtx
$ ./a.out ~/data/web-BerkStan.mtx
$ ...

# Loading graph /home/subhajit/data/web-Stanford.mtx ...
# order: 281903 size: 2312497 {}
# order: 281903 size: 2312497 {} (transposeWithDegree)
# [00405.637 ms; 063 iters.] [0.0000e+00 err.] pagerankSeq
#
# ...
#
# Loading graph /home/subhajit/data/soc-LiveJournal1.mtx ...
# order: 4847571 size: 68993773 {}
# order: 4847571 size: 68993773 {} (transposeWithDegree)
# [12092.729 ms; 051 iters.] [0.0000e+00 err.] pagerankSeq
#
# ...
```

[![](https://i.imgur.com/jUgH24r.png)][sheetp]
[![](https://i.imgur.com/bg2zNx0.png)][sheetp]

<br>
<br>


## References

- [PageRank Algorithm, Mining massive Datasets (CS246), Stanford University](https://www.youtube.com/watch?v=ke9g8hB0MEo)
- [SuiteSparse Matrix Collection]

[SuiteSparse Matrix Collection]: https://sparse.tamu.edu
[pull]: https://github.com/puzzlef/pagerank-push-vs-pull
[CSR]: https://github.com/puzzlef/pagerank-class-vs-csr
[charts]: https://photos.app.goo.gl/owJ8YMMpoQQUqLGx5
[sheets]: https://docs.google.com/spreadsheets/d/1gWzOw_715qpzYxjTvV5ti-lyMcsiqt43Vy9IFyibUGc/edit?usp=sharing
[sheetp]: https://docs.google.com/spreadsheets/d/e/2PACX-1vQjvsrRquyQ0wE1e33Raz3mOYnTRU-hhTbk1nSRPraM1GkgBBxitL5KQjYwGTgpK7lDhD_ZMqs0jYze/pubhtml
