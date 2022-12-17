# Golang HTTP Client

[![Go Report Card](https://goreportcard.com/badge/BRUHItsABunny/gOkHttp)](https://goreportcard.com/report/BRUHItsABunny/gOkHttp)
[![License](http://img.shields.io/badge/license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/BRUHItsABunny/gOkHttp/master/LICENSE)

## Introduction

gOkHttp is HTTP Client written in Golang inspired by Java's (now Kotlin's) [OkHTTP](https://github.com/square/okhttp) and also slightly inspired by Python's [Requests](https://github.com/kennethreitz/requests). 

This library has been written with handling cookies (in-memory, on-disk, encrypted on-disk), headers, parameters, post fields, post multipart bodies, post files and SSL pinning in mind.

* Inspired by okhttp
    * SSL Pinning implementation and ease of using it
* Inspired by requests
    * Response processing (eg: `responses.ResponseText(httpResp)` to return response body as a string)
    * Making requests with headers and parameters as maps (there where in Python it's dicts)

##### Warning

This library is probably not production ready yet, most of the core was coded in under 2 hours at 1 AM. Proceed with caution, this library was made to fit MY needs and therefore may be structured in a weird way or incomplete (feel free to fix it in a pull request).

## Installation

The package can be installed using "go get".

```bash
go get -u github.com/BRUHItsABunny/gOkHttp
```

## Usage

There is a file filled with examples [here](https://github.com/BRUHItsABunny/gOkHttp/blob/master/lib_test.go) and the you ccan find the Go docs [here](https://pkg.go.dev/github.com/BRUHItsABunny/gOkHttp)

## Contributions

Feel free to fork this repository and open up pull requests.

## Todo

* Built in HTTP3 support (as a switch)
* Built in HLS downloader (with its own muxer)
* Redo cookies - and easier access to cookies
