# JA3Transport

[![GoDoc](https://godoc.org/github.com/CUCyber/ja3transport?status.svg)](https://godoc.org/github.com/CUCyber/ja3transport)
[![Go Report Card](https://goreportcard.com/badge/github.com/CUCyber/ja3transport)](https://goreportcard.com/report/github.com/CUCyber/ja3transport)

For a more in-depth look at the library, check out our [blogpost].

## Abstract
JA3 is a method for fingerprinting TLS clients using options in the TLS ClientHello packet like SSL version and available client extensions. At its core, this method of detecting malicious traffic is marginally better than the User-Agent header in HTTP since the client is in control of the ClientHello packet. Currently, there is no tooling available to easily craft ClientHello packets, so the JA3 hash is a great detection mechanism. A team of two members from CU Cyber have created a Go library that makes it easy to mock JA3 signatures.


[blogpost]: https://medium.com/cu-cyber/impersonating-ja3-fingerprints-b9f555880e42
