# Week 2 - Shift Operations

## 1. Experiment Title

**Shift Operations and LED Control**

---

## 2. Experiment Objectives

* Understand shift operations.
* Learn how to use the left shift operator `<<`.
* Learn how to use the right shift operator `>>`.
* Understand comparison operators.
* Understand how to use the AND operator `&`.
* Use loops and conditional statements to control the program.
* Understand how port values change through shift operations.

---

## 3. Experiment Theory

* `<<`: Moves bits to the left.
* `>>`: Moves bits to the right.
* `&`: Performs a bitwise AND operation.
* `==`: Checks whether two values are equal.
* `<=`: Checks whether a value is less than or equal to another value.
* `>=`: Checks whether a value is greater than or equal to another value.
* Shift operations can be used to move a bit through different positions.
* The AND operation can be used with an `if` statement to check whether a specific value has been reached.

---

## 4. Experiment Procedure and Code

### Example 1

Example 1 introduces shift operations and demonstrates how a value such as `0x01` can be shifted to `0x02`.

A delay is used to make the change visible to the human eye.

```c
```

### Example 2

Example 2 demonstrates the execution speed of the microprocessor.

The shift operation happens very quickly, so the intermediate operation cannot be seen by the human eye. The delay allows the final output to remain visible.

```c
```

### Example 3

Example 3 introduces the use of a `do-while` loop to repeatedly execute the program.

```c
```

### Example 4

Example 4 uses the AND operation `&` together with an `if` statement.

The purpose is to check a specific value and make the operation continue repeatedly.

```c
```

### Example 5

Example 5 uses the AND operation to determine whether the desired target value has been reached.

The current `PortInitValue` is compared with `0x80` using the AND operation. When the reference value is obtained, it indicates that the target has been reached.

```c
```

### Example 6

Example 6 uses the same code as Example 5.

The maximum value of `j` is changed from `50000` to `100000` to observe what changes and understand why the change occurs.

```c
```

### Example 7

Example 7 modifies the program so that the movement speed can be adjusted.

The purpose is to understand each line of the code and why each part is used.

```c
```

### Example 8

Example 8 is created by modifying Example 7.

The example continues to use a left shift operation while changing the implementation of the previous example.

```c
```

### Example 9

Example 9 is created by modifying Example 8.

It is compared with Example 4 to understand that the same behavior can be implemented using different approaches.

```c
```

---

## 5. Shift Operation

A shift operation moves the bits of a binary value to the left or right.

For example:

```text
00000011
   << 3
01100000
```

The left shift operator `<<` moves the bits to the left, while the right shift operator `>>` moves the bits to the right.

---

## 6. AND Operation

The AND operator `&` compares each corresponding bit of two values.

| Input | Input | Output |
| ----- | ----- | ------ |
| 0     | 0     | 0      |
| 0     | 1     | 0      |
| 1     | 0     | 0      |
| 1     | 1     | 1      |

It can be used with an `if` statement to check whether a specific value has been reached.

---

## 7. Experiment Results

* Shift operations were used to move values between different bit positions.
* The left shift `<<` and right shift `>>` operators were introduced.
* The AND operator `&` was used to check specific values.
* Loops were used to repeatedly execute operations.
* The program's movement speed could be adjusted.
* Different coding methods can produce the same behavior.

---

## 8. Discussion

In this experiment, I learned how shift operations can be used to move bits between different positions. I also learned how the `<<` and `>>` operators work and how they can be used to control port values.

I learned how the AND operator `&` can be combined with an `if` statement to check whether a specific value has been reached. Loops were also used to make the operation
