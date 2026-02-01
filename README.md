# Golang Practice

## Section 1:
 1. What Go offers, Go vs other languages
 2. Go installation
 3. Compiling and running first Go Program
 4. Go Programming Syntax

### Golang Features

- Fast compilation – very quick build times even for large codebases
- No heavy runtime dependency – produces a single binary with minimal runtime overhead
- Cross-compilation support – build binaries for multiple OS and architectures from one machine
- Built-in concurrency – goroutines and channels make concurrent programming simple and efficient
- Not fully OOP – no classical inheritance; uses structs, interfaces, and composition
- Statically typed language – type safety at compile time, fewer runtime errors
- Very simple language – small syntax with ~25 keywords, easy to learn and maintain

---

### Basic Commands

Run a Go program:
go run hello.go

Build the binary:
go build hello.go

Build and generate a custom output binary:
go build -o app hello.go

Cross-compile for another OS and architecture:
GOOS=linux GOARCH=amd64 go build -o app hello.go

List supported OS and architectures:
go tool dist list

Install binary/executable to GOBIN:
go install hello.go

Install binary from a remote repository:
go install github.com/JitenPalaparthi/urllinter@latest

Compile and link using Go tools (low-level):
go tool compile hello.go
go tool link -o hello.exe hello.o

---

### Go Modules and Packages

Package Types:

1. Standard packages  
   Location: $GOROOT/src/

2. User-defined packages (before Go 1.11)  
   Location: $GOPATH/src/, $GOPATH/pkg/, $GOPATH/bin/

3. Third-party packages  
   Managed using Go Modules

Go Modules (go mod):

- Introduced in Go 1.11
- Used to manage dependencies and versions
- Works outside GOPATH
- Recommended for user-defined and third-party packages

Initialize a module:
go mod init <module-name>


## Go Modules (Very Short)

`go mod init` initializes a Go module and creates a `go.mod` file.

It enables:
- Dependency management
- Versioning
- Working outside GOPATH

Key files:
- `go.mod` → module name, Go version, dependencies
- `go.sum` → dependency checksums

Common commands:
- go mod init
- go mod tidy

In short: Go Modules manage dependencies in modern Go projects.

## Section 2:
 1. Package, Variables and constants, Data types
 2. Functions
 3. If, if-else, switch, for
 4. Array
 5. Slice: underlying array, extract, append, spread, copy
 6. Maps
 7. String, byte, rune, utf-8 encoding

