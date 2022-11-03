*I dont even know if this go snippet works lmao*

### hi
I need help


```go
package beakeyz

import(
    "fmt"
)

type Beakeyz struct{
    Id            int
    FavoriteLangs []string
    Learning      []string
    Despises      []string
    Loves         []string
}

// helper function in a readme. Noice
func getAttribute(a []string) string{
    var val string
    for index, value := range(a){
        if index == len(a) - 1{
            val = append(val, "and " + value)
        }else{
            val = append(val, value + ", ")
        }
    }
    return val
}

// epic
func (self Beakeyz) PrintSelf(){
    fmt.Printf("My age is: %s\n", self.Id)
    
    fmt.Printf("My favorite languages are: %s\n", getAttribute(self.FavoriteLangs))
    fmt.Printf("I'm currently learning: %s\n", getAttribute(self.Learning))
    fmt.Printf("I fucking hate: %s\n", getAttribute(self.Despises))
    fmt.Printf("I absolutely love: %s\n", getAttribute(self.Loves))
}

// main function
func main(){
    var me Beakeyz = &Beakeyz{
        Id: 16,
        FavoriteLangs: []string{"go", "java", "c++/c"},
        Learning: []string{"C#", "Rust", "(opperating) systems", "assembly", "networking protocols (fuck me)", "life"},
        Despises: []string{"javascript, yuck", "social interaction. Yes, im that guy"},
        Loves: []string{"skiing", "programming"}
    }

    me.PrintSelf()
}

```
