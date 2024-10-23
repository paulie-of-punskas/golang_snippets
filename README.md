## Notes is Golang mokymosi

### Kalbos ypatumai
- nesikompiliuos, jeigu importuota "package" bus nepanaudota
- kap paleist: `go run filename.go`
- viskas yra package
- `:=` operatorus gali but panaudotas tik funcijos viduje
- everything capitalized is exported (pvz. funkcija, gali but panaudota kitos funkcijos)

### Funkcijos
- `func main(int, []string) int` (function takes integer, slice of strings and returns an int)
- `func main(a, b, c int) int` (function takes integers a, b, c and returns an integer)

#### fmt.Printf
- formatai: golang.org/pkg/fmt
`fmt.Printf("xx: %8T %v\n", xx, xx)`
`fmt.Printf("xx: %8T %[1]v\n", xx)`

### Composite types (array, slice ...)
- string
- array: `[4]int` 
    - size of arrays needs to be declared 
- slice: variable length array (pvz. []int)
    - not comparable 
- map: `map[string]int` (key type = string, value type = int), panasiai kaip Java
	- `make(map[string]int)` -- `make` creates a hash table in the background

### if/else/ok
- `if w, ok := p["the"]; ok { ... }`
    - declare variables `w`, `ok`
    - `(...); ok {` is a boolean if statement
    - "if 'the' exists, the do something"
 
### control statements

