interval-tree-1d
================
A simple 1D interval tree.  Supports O(log(n)) amortized updates and O(log(n)) queries.

# API

```javascript
var createIntervalTree = require("interval-tree-1d")
```

## Constructor

### `var tree = createIntervalTree(intervals)`
Constructs an interval tree given a list of intervals

## Properties

### `tree.count`
Returns the number of items in the tree

### `tree.intervals`
Returns a list of all the intervals in the tree

### `tree.insert(interval)`
Adds an interval to the tree

### `tree.remove(interval)`
Removes an interval from the tree

### `tree.queryPoint(p, visit(interval))`
Visits all intervals containing the point p

### `tree.queryInterval(lo, hi, visit(interval))`
Returns all intervals which intersect the interval `[lo, hi]`

# Credits
(c) 2013 Mikola Lysenko. MIT License