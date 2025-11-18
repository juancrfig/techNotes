***

It's a package from the *standard library* 

***
### Basic Methods
```Go
// Creates a new base context
ctx := context.Background()
//                    parent   key     value
ctx = context.WithValue(ctx, "name", "Juanes")

// Retrieves a value from a context by using its key
v := ctx.Value("name")  // v == "Juanes"
```
***