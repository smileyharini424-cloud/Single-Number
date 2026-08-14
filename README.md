# Single Number

## Explanation

The Single Number problem requires finding the element that appears only once in an array where every other element appears exactly twice.

The program uses the **XOR** operation to find the unique element efficiently.

## Problem Statement

Given a non-empty array of integers `nums`, every element appears twice except for one element that appears only once. Find and return the element that appears only once.

## Features

* Finds the unique element
* Uses XOR operation
* Does not require an additional data structure
* Traverses the array only once
* Efficient solution

## How It Works

The program starts with:

```text
result = 0
```

Each element is then XORed with `result`.

The important XOR properties are:

```text
a ^ a = 0
a ^ 0 = a
```

Therefore, all duplicate numbers cancel each other out and the number that appears only once remains.

For example:

```text
4 ^ 1 ^ 2 ^ 1 ^ 2
```

The duplicate values cancel:

```text
4
```

So the answer is `4`.

## Technologies Used

* Arrays
* Loops
* XOR operation
* Methods
* Conditional logic

## Data Structure Used

The program uses an integer array.

No additional data structure is required.

## Methods Used

### singleNumber()

Uses XOR to find and return the element that appears only once.

### main()

Creates the sample input, calls `singleNumber()`, and displays the result.

## Program Flow

```text
Start
↓
Read array
↓
Set result to 0
↓
Traverse array
↓
Apply XOR with each element
↓
Duplicate values cancel
↓
Unique value remains
↓
Return result
↓
Display result
↓
End
```

## Sample Input

```text
nums = [4, 1, 2, 1, 2]
```

## Sample Output

```text
Single Number: 4
```

## Time Complexity

```text
O(n)
```

The array is traversed once.

## Space Complexity

```text
O(1)
```

Only one extra variable is used.

## Key Learning

This problem teaches how the XOR operation can be used to find a unique element when every other element appears exactly twice.

## File Location

```text
Arrays/SingleNumber.java
```

## Repository Structure

```text
Single-Number/
├── README.md
└── Arrays/
    └── SingleNumber.java
```

## Author

**V.Harini**
