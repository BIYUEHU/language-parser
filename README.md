# Some Language

> Developing...

A Functional and Dependent Type Programming Language Base on Rust.

## Features

- Modern Syntax
- Functional Programming
- Dependent Types
- The First-Class Type
- Parsing and Type Checking
- Many targets
- Simple, safe and Fast

## Demo

```txt
let foo = 1
foo = 2 // Error
let foo = "Hello, FP!"
let foo: Char = 'X'
let foo: Bool = False
let foo: Float = 3.1415926

type Bool = True | False
type List: Kind -> Kind = <T> Cons(T, List<T>) | Nil
type String = List<Char>
type String = [Char]

let fruits: List<String> = Cons("Apple", Cons("Banana", Cons("Pear", Nil)))
let fruits: [String] = ["Apple", "Banana", "Pear"]

let add: Int -> Int -> Int = x => y => x + y
let add: Int -> Int -> Int = (x, y) => x + y
let add = (x: Int, y: Int) -> Int => x + y

let fibonacii: Int -> Int =
 | 1 => 1
 | 2 => 1
 | x => fibonacii(x - 1) + fibonacii(x - 2)
let fibonacii: Int -> Int = x => match x {
    | 1 => 1
    | 2 => 1
    | x => fibonacii(x - 1) + fibonacii(x - 2)
}

let handle_score = (x: Int) =>
    if x > 100 || x < 0 then "Fake"
    else if x == 100 then "Best"
    else if x > 90 then "Excellent"
    else if x > 70 then "Good"
    else if x > 60 then "Not bad"
    else if x > 40 then "Bad"
    else "Shit"

let bar = (
    let x = 20, y = 30
    in x + y ^ 2 * 2 / 5 - 5 % 1
)
let bar = {
    let x = 20, y = 30
    x + y ^ 2 * 2 / 5 - 5 % 1
}

// Token

```
