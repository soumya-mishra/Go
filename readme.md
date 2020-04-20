## GO
- statically types
- compiled language , Fast compilation 
- memory safety
- grabage collection
- structural typing
- concurrency - builtin 
- variable initialization - x:= 0  or var x = 0

package main

  import (
    "fmt"
    "time"
    )
    
 func manin(){
 
    fmt.Println("1st prog")
  
    fmt.Println("time is time.now())
  
 }

import package "fmt" "math" 

func main(){

    fmt.Println(math.Pi)
    
}
   
- function as func 

package main

import "fmt"

func add(x int, y int) int {

	return x + y
	
}

func main() {

	fmt.Println(add(42, 13))
}


- x,y int  also possible in func 
- multiple return 
 
 package main
 import "fmt"
  
  func swap(x,y string) (string,string){
   
     return y, x
 
 }
  
  func main() {
  
  a,b:= swap("hello" ,"world")
 
  fmt.Println(a, b)
  

- Named return values
  
  package main

import "fmt"

func split(sum int) (x, y int) {
	x = sum * 4 / 9
	y = sum - x
	return
}

func main() {
	fmt.Println(split(17))
}

- variable declaration 
  var c, python, java bool
  
- variable with initializer 
  var i, j int = 1, 2
  
 - var c, python, java = true, false, "no!" 
 - Inside a function, the := short assignment statement can be used in place of a var declaration with implicit type.
 - Outside a function, every statement begins with a keyword (var, func, and so on) and so the := construct is not available.
 - bool string int int8 int16 int32 int64 
 - uint uint8 uint16 uint32 uint64 uintptr
 - byte
 - rune - alias for int32
 - float32 float64
 - complex64 complex128
 - Type conversion
 	- var i int = 42
	- var f float64 = float64(i)
 	- var u uint = uint(f)
 
  - Default type
	- i := 42           // int
	- f := 3.142        // float64
	- g := 0.867 + 0.5i // complex128

- const name = "sss"
- Constants cannot be declared using the := syntax.

- FOR 
for i := 0; i < 10; i++ {

		sum += i
	}



for ; sum < 1000; {

		sum += sum
	}

for sum < 1000 {

		sum += sum
	}


- if x < 0 {

  }
 
 - 
 if v := math.Pow(x, n); v < lim {
		
		return v
		
	} else {
		
		fmt.Printf("%g >= %g\n", v, lim)
	}

- switch

switch os := runtime.GOOS; os {

	case "darwin":
	
		fmt.Println("OS X.")
		
	case "linux":
	
		fmt.Println("Linux.")
		
	default:
	
		// freebsd, openbsd,
		
		// plan9, windows...
		
		fmt.Printf("%s.\n", os)
	}

-  Switch with no condition is true

switch {
	
	case t.Hour() < 12:
		
		fmt.Println("Good morning!")
	
	case t.Hour() < 17:
		
		fmt.Println("Good afternoon.")
	
	default:
		
		fmt.Println("Good evening.")
	}

- defer 

package main

import "fmt"

func main() {
	
	defer fmt.Println("world")

	fmt.Println("hello")
}

o/p : hello  world

- Deferred function calls are pushed onto a stack. When a function returns, its deferred calls are executed in last-in-first-out order.

- pointer
- structs
type Vertex struct {
	x int
	y int
	}
- array -> var a [10] int
- 
