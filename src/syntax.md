# Syntax


## Variables 

### Assignment

`a := 3` assigns the int `3` to var `a`


## Collections


### Arrays

Arrays have a defined length.  Elements can be defined at declaration or after. 

Declare array and add elements after:

```go
var myArray [2]string
    myArray[0] = "foo"
    myArray[1] = "bar"
```

Declare array and add elements at time of declaration: 

```go
myArray  := [2]string{"foo", "bar"}
```


### Slices 

Most array programming in Go is done with slices rather than simple arrays.

You can put more items into a slice than what it was initialized for.

#### Demonstration:  

```go
// Create the slice
mySlice := make([]string, 0)

myString := "FooBar"

//To append an item to the slice:
mySlice := append(mySlice, myString)
```


