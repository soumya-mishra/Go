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
