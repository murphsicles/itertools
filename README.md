# @std/itertools — Extra Iterator Adaptors for Zeta

Auto-converted from [itertools](https://crates.io/crates/itertools) v0.14.0 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- **Chaining/zipping** — `chain`, `zip`, `izip!`, `interleave`, `interleave_shortest`, `intersperse`
- **Filtering** — `filter`, `filter_map`, `filter_ref`, `peek_nth`, `take_while_ref`
- **Grouping** — `group_by`, `chunks`, `chunk_by`, `coalesce`, `dedup`, `unique`, `unique_by`
- **Sorting** — `sorted`, `sorted_by`, `sorted_unstable`, `k_smallest`, `merge`, `merge_by`, `merge_join_by`
- **Partitioning** — `partition`, `partition_map`, `split`, `splitn`, `rciter`
- **Combinatorics** — `combinations`, `permutations`, `powerset`, `cartesian_product`, `circular_tuple_windows`
- **Aggregation** — `minmax`, `min_set`, `max_set`, `all_equal`, `counts`, `fold`, `reduce`, `tree_fold`
- **Adaptors** — `map`, `map_into`, `map_ok`, `filter_ok`, `flatten_ok`, `update`, `foreach`, `collect`

## Usage
```zeta
use @std/itertools::Itertools;

let data = vec![1, 2, 3, 4, 5];
let result: Vec<_> = data.iter()
    .filter(|x| x > 2)
    .sorted()
    .unique()
    .collect();
```

## Stats: ~5,334 lines, 0 unsupported items

## License: MIT