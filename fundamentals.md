# Go Fundamentals Concepts:
## Identifiers in Go:
Example:
```
package main
import "fmt"

func main() {

 var name = "Hello World"
  
}
```
There is total of three identifiers available in the above example:

main: Name of the package
main: Name of the function
name: Name of the variable
### Keywords:
break, case, chan, const, continue, default, defer, else, fallthrough, for, func, go, goto, if
import, interface, map, package, range, return, select, struct, switch, type, var 
### Datatypes:
Data types specify the type of data that a valid Go variable can hold. In Go language, the type is divided into four categories which are as follows:

***Basic type:*** Numbers, strings, and booleans come under this category.
***Aggregate type:*** Array and structs come under this category.
***Reference type:*** Pointers, slices, maps, functions, and channels come under this category.
***Interface type***

***Integers type:***
1. int8	8-bit signed integer.
2. int16	16-bit signed integer.
3. int32	32-bit signed integer.
4. int64	64-bit signed integer.
5. uint8	8-bit unsigned integer.
6. uint16	16-bit unsigned integer.
7. uint32	32-bit unsigned integer.
8. uint64	64-bit unsigned integer.
9. int	Both int and uint contain same size, either 32 or 64 bit.
10. uint	Both int and uint contain same size, either 32 or 64 bit.
11. rune	It is a synonym of int32 and also represent Unicode code points.
12. byte	It is a synonym of uint8.
13. uintptr	It is an unsigned integer type. Its width is not defined, but its can hold all the bits of a pointer value.

***Example:***
```
// Go program to illustrate
// the use of integers
package main
import "fmt"
		
func main() {
	
	// Using 8-bit unsigned int
	var X uint8 = 225
	fmt.Println(X, X-3)
	
	// Using 16-bit signed int
	var Y int16 = 32767
	fmt.Println(Y+2, Y-2)
}

```
***loating-Point Numbers***
1. float32	32-bit IEEE 754 floating-point number.
2. float64	64-bit IEEE 754 floating-point number.

***Example:***

```
// Go program to illustrate
// the use of floating-point
// numbers
package main
import "fmt"
		
func main() {
	a := 20.45
	b := 34.89
	
	// Subtraction of two
	// floating-point number
	c := b-a
	
	// Display the result
	fmt.Printf("Result is: %f", c)
	
	// Display the type of c variable
	fmt.Printf("\nThe type of c is : %T", c)
}

```
### Variables  in GO Language
***Variable declaration in GO.***
```
// Go program to illustrate
// concept of variable
package main

import "fmt"

func main() {

// Variable declared and
// initialized without the
// explicit type
var myvariable1 = 20
var myvariable2 = "Hello World"
var myvariable3 = 34.80

// Display the value and the
// type of the variables
fmt.Printf("The value of myvariable1 is : %d\n",
								myvariable1)
									
fmt.Printf("The type of myvariable1 is : %T\n",
								myvariable1)
	
fmt.Printf("The value of myvariable2 is : %s\n",
									myvariable2)
										
fmt.Printf("The type of myvariable2 is : %T\n",
								myvariable2)
	
fmt.Printf("The value of myvariable3 is : %f\n",
									myvariable3)
										
fmt.Printf("The type of myvariable3 is : %T\n",
								myvariable3)
	
}

```

***Using short variable declaration:***
```

// Go program to illustrate
// concept of variable
package main
import "fmt"

func main() {

// Using short variable declaration
myvar1 := 39
myvar2 := "Hello World"
myvar3 := 34.67

// Display the value and type of the variables
fmt.Printf("The value of myvar1 is : %d\n", myvar1)
fmt.Printf("The type of myvar1 is : %T\n", myvar1)

fmt.Printf("\nThe value of myvar2 is : %s\n", myvar2)
fmt.Printf("The type of myvar2 is : %T\n", myvar2)

fmt.Printf("\nThe value of myvar3 is : %f\n", myvar3)
fmt.Printf("The type of myvar3 is : %T\n", myvar3)
}


```

***Constants- Go Language***

```
package main

import "fmt"

const PI = 3.14

func main()
{
	const GFG = "Hello World"
	fmt.Println("Hello", GFG)

	fmt.Println("Happy", PI, "Day")

	const Correct= true
	fmt.Println("Go rules?", Correct)
}

```
