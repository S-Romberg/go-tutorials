### Pointers
``` 	
    x := 15
	a := &x // memory address
	fmt.Println(a) // memory address
	*a = 5  // 5, value it's pointing to
	fmt.Println(*a) // 5
	fmt.Println(x) // 5
```


### General

`nil === null`


```
import "net/http"

func index_handler(w http.ResponseWriter, r *http.Request) {
	fmt.Fprintf(w, "Whoa, Go is neat")
}

func about_handler(w http.ResponseWriter, r *http.Request) {
	fmt.Fprintf(w, "Whoa, this is about")
}

func main() {
	http.HandleFunc("/", index_handler)
	http.HandleFunc("/about/", about_handler)
	http.ListenAndServe(":8000", nil)
}
```

### Structs


