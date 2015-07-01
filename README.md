# go-image-png

This is a fork of the Go standard library "image/png" with a few niceties.

## Features

- Support for simple Truecolor transparency (where the tRNS chunk is [encoded with one RGB value that is fully transparent](http://www.w3.org/TR/PNG-Chunks.html)). There is currently an [open review](https://go-review.googlesource.com/#/c/11613/) for this feature change that is pending review for Go 1.6.

## Use

Just import as you would other `image` packages. `image.Decode` and `image.Encode` should work out of the box.

```golang
import _ "github.com/mduvall/go-image-png/png"
```
