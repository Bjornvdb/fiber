[![Fiber Logo](https://i.imgur.com/zzmW4eK.png)](https://fiber.wiki)

[Express](https://github.com/expressjs/express) inspired web framework build on [Fasthttp](https://github.com/valyala/fasthttp) for [Go](https://golang.org/doc/).  
Designed to ease things up for fast development with zero memory allocation and performance in mind.

[![](https://img.shields.io/github/release/gofiber/fiber)](https://github.com/gofiber/fiber/releases)
[![](https://img.shields.io/badge/godoc-reference-blue.svg?longCache=true&style=flat)](https://pkg.go.dev/github.com/gofiber/fiber?tab=doc)
![](https://img.shields.io/badge/coverage-84%25-brightgreen.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/go-100%25-brightgreen.svg?longCache=true&style=flat)
![](https://img.shields.io/badge/goreport-A+-brightgreen.svg?longCache=true&style=flat)
[![](https://img.shields.io/badge/gitter-chat-brightgreen.svg?longCache=true&style=flat)](https://pkg.go.dev/github.com/gofiber/fiber?tab=doc)

```go
package main

import "github.com/gofiber/fiber"

func main() {
  app := fiber.New()

  app.Get("/", func(c *fiber.Ctx) {
    c.Write("Hello, World!")
  })

  app.Listen(3000)
}
```

## Benchmarks

These tests are performed by [TechEmpower](https://github.com/TechEmpower/FrameworkBenchmarks) and [Go Web](https://github.com/smallnest/go-web-framework-benchmark). If you want to see all results, please visit our [wiki#benchmarks](https://fiber.wiki/#benchmarks).
<p float="left" align="middle">
  <img src="https://fiber.wiki/static/benchmarks/benchmark-pipeline.png" width="49%" />
  <img src="https://fiber.wiki/static/benchmarks/benchmark_alloc.png" width="49%" /> 
</p>

## Installation

Before installing, [download and install Go](https://golang.org/dl/).
Go `1.11` or higher is required.

Installation is done using the
[`go get`](https://golang.org/cmd/go/#hdr-Add_dependencies_to_current_module_and_install_them) command:

```bash
go get github.com/gofiber/fiber
```

## Features

* Robust routing
* Serve static files
* Extreme performance 
* Low memory footprint
* Express API endpoints
* Middlewares & `Next` support
* Rapid server-side programming
* [Extended API documentation](https://fiber.wiki/)


## Philosophy

People switching from [Node.js](https://nodejs.org/en/about/) to [Go](https://golang.org/doc/) often end up in a bad learning curve to start building their webapps, this project is meant to **ease** things up for **fast** development, but with **zero memory allocation** and **performance** in mind.

## Examples


## License

`gofiber/fiber` is free and open-source software licensed under the [MIT License](https://github.com/gofiber/fiber/master/LICENSE).