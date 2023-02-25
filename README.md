# Redis Distributed Locks Example in Go

Just a simple example highlighting how to use distributed locks in Redis with Go. If you want to learn more about distributed locks and how they work I recommend reading [this](https://redis.io/topics/distlock) article and I wrote a [blog post](https://dev.to/jdvert/handling-mutexes-in-distributed-systems-with-redis-and-go-5g0d) about it too.

## Getting Started

### Prerequisites

- [Redis](https://redis.io/) 
- [Go](https://golang.org/)


### Installing

```bash
go mod download
```

## Running 
    
```bash
go run main.go
```

Example output:

```bash
First lock acquired!
Could not get a second lock which is as expected this is where you would force the request out.
Still could not get the third lock since the first lock is still set.
First lock released!
Forth Lock acquired!
Forth Lock released!
```


