# Collections

## Arrays

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


## Slices 

Most array programming in Go is done with slices rather than simple arrays.

You can put more items into a slice than what it was initialized for.

### Demonstration:  

```go
// Create the slice
mySlice := make([]string, 0)

myString := "FooBar"

//To append an item to the slice:
mySlice := append(mySlice, myString)
```


## Iteration

https://stackoverflow.com/questions/7782411/is-there-a-foreach-loop-in-go

```go
for index, element := range someSlice {
    // index is the index where we are
    // element is the element from someSlice for where we are
}

for _, element := range someSlice {
    // element is the element from someSlice for where we are
}
```


## Maps

Maps are the associative array of the Go world though they are typed. 

### Map Literals

Maps can be created and assigned in one operation using a literal

```go
person := map[string]string {
	"name": "Hugh Smith",
	"occupation": "Insurance Salesman"
}
```


### Making a Map

You can also make a map and add elements to it after creation. 

```go
var m map[string]Vertex

func main()  {
	person = make(map[string]string) 
	person["name"] = "Hugh Smith"
	person["occupation"] = "Insurance Salesman"
}
```
