# Go Map Access Panic

This repository demonstrates a common error in Go: panicking due to accessing a nil map.  The `bug.go` file contains the erroneous code, while `bugSolution.go` provides a corrected version.

## Problem

In Go, attempting to access a map element before checking if the map itself is `nil` will result in a runtime panic. This can be difficult to track down, especially in larger applications.

## Solution

Always check for `nil` before accessing map elements. Use the `if` statement or a conditional expression to ensure that the map exists before attempting access.  A good practice is to initialize the map explicitly.