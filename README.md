Sample based on [Golang/WebAssembly(https://github.com/golang/go/wiki/WebAssembly)

# Build

```shell
GOOS=js GOARCH=wasm go build -o main.wasm
```

# Run

```shell
goexec 'http.ListenAndServe(":8080", http.FileServer(http.Dir(".")))'
```

http://localhost:8080/index.html
