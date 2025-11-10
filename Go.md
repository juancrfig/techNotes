***

It's a ***statically typed***, ***call-by-value*** and [[compilation|compiled]] [[programming language]] with ***implicit interfaces***. 
Each programs includes a small amount of extra code called the [[Go Runtime]].

***
## Data Types

**Signed Integers**
- `int8 int16 int32 int64` 
**Unsigned Integers**
- `uint8 uint16 uint32 uint64`
**Signed Decimals**
- `float32 float64`
The number at the end represents *bits*. `int` and `uint` refer to their respective 32 or 64-bit sizes, depending on the user's environment. 

***
# Dictionary

- **Package:** A directory containing source files, allows organization, encapsulation and code reusability. 
- **Module:** The highest-level container of source  code. It's defined by the presence of the file `go.mod` at the directory's root. 
- **Interface:** It's a collection of method signatures. A type *implements* an interface if it has methods that match the interface's method signatures.

***

### Algorithms to build

- Bubble sort
- Binary Search
- Merge sort
- Selection Sort
- Quicksort
- Insertion Sort

### Data Structures

- [[Linked List]]
- Stack
- Queue
- Binary Tree / BST

***
## Important Facts

- *`const` variables must be known at compile time*.
- The data type `rune` is an alias for `int32`. An *32-bits* number is big enough to represent any *Unicode* symbol. 
- When **maps** and **slices** are passed as argument in a function, they are passed as ***reference***.
- Trying to deference a *nil* pointer will cause a runtime error that crashes the program (panic). 

***
## Syntax

##### Initial Statement of an If block
```Go
if INITIAL_STATEMENT; CONDITION {
	// some code
}
```

***

## Errors

Go programs express errors with `error` values. An **`Error`** is any type that implements the *built-in* error interface. 

```go
type error interface {
	Error() string
}
```

***

## Stuff to Investigate Later

>>>Interestingly, local non-pointer variables are generally faster to pass around than pointers because they're stored on the [stack](https://computersciencewiki.org/index.php?title=Stack_memory), which is faster to access than the [heap](https://computersciencewiki.org/index.php/Heap_memory). Even though copying is involved, the stack is so fast that it's no big deal

[article about it](https://blog.boot.dev/golang/pointers-faster-than-values/?_gl=1*ghg53w*_ga*MTg4MDQ0NTQ1My4xNzYxMzM4NTY4*_ga_M7P2PBGN8N*czE3NjI3MzAyODAkbzgxJGcxJHQxNzYyNzM5ODA3JGozNSRsMCRoODQ5MDA5OTg1JGR2VlcwOUxzOGVGTUN0dkFBVWM0eFNoVDFlR1ZTUDliU2V3*_gcl_au*MTM0NDYxNDU0MS4xNzYxMzM4NTY4LjE2OTAxODQzMzAuMTc2MjczOTEyMy4xNzYyNzM5MTIy)

***

>>>The dependency arrow should always point **inward** (apps depend on packages), never **outward** (packages depend on apps).

***

