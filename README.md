# wasm_test
Having a go a compiling a WASM module for a basic website.

## Build WASM File

Uses GO Version 1.14.4
Consider using GVM (Go Version Manager) to simplify the handling of Go versions.

```bash
GOOS=js GOARCH=wasm go build -o main.wasm
```

```bash
goexec 'http.ListenAndServe(`:8080`, http.FileServer(http.Dir(`.`)))'
```