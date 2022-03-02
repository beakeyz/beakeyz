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
            langs = append(langs, value + ", ")
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
        Learning: []string{"C#", "assembly", "networking (fuck me)", "life"},
        Despises: []string{"javascript (sorry :/ )", "libraries", "social interaction (ew)"},
        Loves: []string{"skiing", "programming (ofc)", "golang (bae)", "boobies (im down bad, okay?)"}
    }

    me.PrintSelf()
}

```

*I dont even know if this go snippet works lmao*

### 🤗 Hello good person reading my readme 🤗

As you can see I am a _special_ ❄️snowflake❄️
