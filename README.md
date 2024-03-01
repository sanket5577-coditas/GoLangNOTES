# GoLangNOTES


## Topic 1: Variables and Constants

### Variables:

In Go, variables are like containers that hold information. They have a type and can be assigned values. Let's explore the declaration and assignment of variables:

```go
var age int     // Declaration
age = 25        // Initialization

name := "John"  // Shorthand declaration and initialization
```

- **Declaration:** Reserving space in memory for a variable. In our example, `var age int` reserves space for an integer named `age`.
  
- **Initialization:** Giving a variable its initial value. `age = 25` assigns the value `25` to the variable `age`.
  
- **Shorthand:** The `:=` operator declares and initializes a variable in one go. `name := "John"` is equivalent to `var name string` followed by `name = "John"`.

### Constants:

Constants are like variables, but their values cannot be changed after assignment. They are useful for values that should remain constant throughout the program:

```go
const pi = 3.14
```

Here, `pi` is a constant with a value of `3.14`. Once set, you can't later do `pi = 3.14159`. Constants are handy for things like mathematical values that shouldn't change.

#### Key Takeaways:

- **Variables:** Used for storing data that can change during the execution of a program.
  
- **Constants:** Used for values that should not change.

---

## Topic 2: Data Types

### Basic Data Types:

#### Integer:

Integers represent whole numbers. They can be of different sizes, such as `int8`, `int16`, `int32`, and `int64`, indicating the number of bits they use.

```go
var num int      // Declaration
num = 42         // Initialization
```

#### Floating-point:

Floating-point numbers represent real numbers (those with a fractional part), and they come in two sizes, `float32` and `float64`.

```go
var pi float64   // Declaration
pi = 3.14159     // Initialization
```

#### String:

Strings hold sequences of characters. They are immutable, meaning their values cannot be changed once assigned.

```go
name := "Alice"
```

#### Boolean:

Booleans represent true or false values.

```go
isTrue := true
```

### Complex Data Types:

#### Struct:

A struct is a composite data type that groups together variables (fields) under a single name.

```go
type Person struct {
    Name string
    Age  int
}

person := Person{Name: "Alice", Age: 30}
```

#### Array:

An array is a fixed-size collection of items of the same type.

```go
var numbers [3]int
numbers[0] = 1
numbers[1] = 2
numbers[2] = 3
```

#### Slice:

A slice is a dynamic and flexible array. It can grow or shrink.

```go
slice := []int{1, 2, 3, 4, 5}
```

#### Map:

A map is a collection of key-value pairs.

```go
m := make(map[string]int)
m["one"] = 1
m["two"] = 2
```

#### Key Takeaways:

- **Basic Data Types:** Integer, floating-point, string, boolean.
  
- **Complex Data Types:** Struct, array, slice, map.

---

## Topic 3: Control Structures (if-else and for loops)

### If-Else Statements:

If-else statements allow your program to make decisions. They execute a block of code if a condition is true, and another block if it's false.

```go
if x > 10 {
    fmt.Println("x is greater than 10")
} else if x == 10 {
    fmt.Println("x is equal to 10")
} else {
    fmt.Println("x is less than 10")
}
```

Here, `x > 10` is the condition. If it's true, the first block executes. If not, it checks the next condition, and so on.

### For Loops:

For loops allow you to repeat a block of code multiple times.

```go
for i := 0; i < 5; i++ {
    fmt.Println(i)
}
```

- **Initialization (`i := 0`):** Setting up the loop variable.
  
- **Condition (`i < 5`):** The loop will keep running as long as this condition is true.
  
- **Post statement (`i++`):** Executed after each iteration.

#### Key Takeaways:

- **If-Else:** For decision-making based on conditions.
  
- **For Loops:** For executing a block of code repeatedly.

---
