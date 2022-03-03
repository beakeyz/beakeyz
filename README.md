*I dont even know if this go snippet works lmao*

### 🤗 Hello good person 🤗
As you can see I am in need of _special_ mental treatment 


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
    fmt.Sprintf("My age is: %s", self.Id)
    
    fmt.Sprintf("My favorite languages are: %s", getAttribute(self.FavoriteLangs))
    fmt.Sprintf("I'm currently learning: %s", getAttribute(self.Learning))
    fmt.Sprintf("I fucking hate: %s", getAttribute(self.Despises))
    fmt.Sprintf("I absolutely love: %s", getAttribute(self.Loves))
}

// main function
func main(){
    var me Beakeyz = &Beakeyz{
        Id: 16,
        FavoriteLangs: []string{"go", "java", "c++/c"},
        Learning: []string{"C#", "Rust", "(opperating) systems", "assembly", "networking (fuck me)", "life"},
        Despises: []string{"javascript (sorry :/ )", "packages/libraries", "social interaction"},
        Loves: []string{"skiing", "programming (ofc)", "golang", "boobies (im down bad, okay?)"}
    }

    me.PrintSelf()
}

```
