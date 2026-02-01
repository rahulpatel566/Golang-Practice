# Golang Practice

## Day 1

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
