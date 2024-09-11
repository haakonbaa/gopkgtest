# Go subdir module example

to use the module, run
```
go mod init 'somemodule'
```

add the following ```main.go``` file.
```go
package main                                                                                                      
                                                                                    
import (                                                                            
    "fmt"                                                                           
                                                                                    
    "github.com/haakonbaa/gopkgtest/somepkg"                                        
)                                                                                   
                                                                                    
func main() {                                                                       
    fmt.Println("Hello World")                                                      
    somepkg.SomePKG()                                                               
}
```

and run

```
go mod tidy
go run main.go
```


