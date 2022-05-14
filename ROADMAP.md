# Dev Goal


Make package compatible with non-Markovian general case.
E.g.
```
>>> cost_to_go = CostToGo(prop, K, markovian=False)
```
will lead to slices of `cost_to_go` having reference to `cost_to_go`, thereby knowing
about the original problems length.
Then, allow only first control to be optimized for every slice, and everything should work out.