# This is a frozen version of goinsta v1

> Unofficial Instagram API for Golang

[![Build Status](https://travis-ci.org/kozimon0204/goinsta.svg?branch=master)](https://travis-ci.org/kozimon0204/goinsta) [![GoDoc](https://godoc.org/github.com/kozimon0204/goinsta?status.svg)](https://godoc.org/github.com/kozimon0204/goinsta) [![Go Report Card](https://goreportcard.com/badge/github.com/kozimon0204/goinsta)](https://goreportcard.com/report/github.com/kozimon0204/goinsta) [![Coverage Status](https://coveralls.io/repos/github/kozimon0204/goinsta/badge.svg?branch=master)](https://coveralls.io/github/kozimon0204/goinsta?branch=master)

## Features

- **Like Instagram mobile application**. Goinsta is very similar to Instagram official application.
- **Simple**. Goinsta is made by a lazy programmer!
- **Backup methods**. You can use `store` package to export/import `goinsta.Instagram` struct.
- **No External Dependencies**. Goinsta will not use any Go packages outside of the standard library.

## New Version !

We are working on `v2` branch , Try it and tell us your suggestions.

## Installation

`go get -u -v github.com/kozimon0204/goinsta`

Or

`go get gopkg.in/kozimon0204/goinsta.v1`

and then

`import "gopkg.in/kozimon0204/goinsta.v1"`

## Example

```go
package main

import (
	"fmt"

	"github.com/kozimon0204/goinsta"
)

func main() {
	insta := goinsta.New("USERNAME", "PASSWORD")

	if err := insta.Login(); err != nil {
		fmt.Println(err)
		return
	}

	defer insta.Logout()

	...
}
```

- [**More Examples**](https://github.com/kozimon0204/goinsta/tree/master/_examples)

## Legal

This code is in no way affiliated with, authorized, maintained, sponsored or endorsed by Instagram or any of its affiliates or subsidiaries. This is an independent and unofficial API. Use at your own risk.

## Contributors :heart:

| [<img src="https://avatars2.githubusercontent.com/u/10146748?v=4&s=460" width="100px;"/><br /><sub>themester 💎</sub>](https://github.com/themester) | [<img src="https://avatars1.githubusercontent.com/u/20666846?s=460&v=4" width="100px;"/><br /><sub>jaynagpaul 💎</sub>](https://github.com/jaynagpaul) |     [<img src="https://avatars1.githubusercontent.com/u/943597?v=4&s=460" width="100px;"/><br /><sub>icholy</sub>](https://github.com/icholy)     |         [<img src="https://avatars3.githubusercontent.com/u/377909?v=4&s=460" width="100px;"/><br /><sub>rakd</sub>](https://github.com/rakd)         | [<img src="https://avatars1.githubusercontent.com/u/14817537?v=4&s=460" width="100px;"/><br /><sub>kemics</sub>](https://github.com/kemics) |  [<img src="https://avatars0.githubusercontent.com/u/4770842?v=4&s=460" width="100px;"/><br /><sub>sklinkert</sub>](https://github.com/sklinkert)   | [<img src="https://avatars1.githubusercontent.com/u/3836912?v=4&s=460" width="100px;"/><br /><sub>vitaliikapliuk</sub>](https://github.com/vitaliikapliuk) |
| :--------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------: |
|      [<img src="https://avatars0.githubusercontent.com/u/1041407?v=4&s=460" width="100px;"/><br /><sub>glebtv</sub>](https://github.com/glebtv)      |      [<img src="https://avatars1.githubusercontent.com/u/7801927?v=4&s=460" width="100px;"/><br /><sub>neetkee</sub>](https://github.com/neetkee)      |   [<img src="https://avatars1.githubusercontent.com/u/13871989?v=4&s=460" width="100px;"/><br /><sub>daciwei</sub>](https://github.com/daciwei)   | [<img src="https://avatars0.githubusercontent.com/u/321920?v=4&s=460" width="100px;"/><br /><sub>aaronarduino</sub>](https://github.com/aaronarduino) |    [<img src="https://avatars3.githubusercontent.com/u/437741?v=4&s=460" width="100px;"/><br /><sub>tggo</sub>](https://github.com/tggo)    | [<img src="https://avatars3.githubusercontent.com/u/10453357?v=4&s=460" width="100px;"/><br /><sub>Albina-art</sub>](https://github.com/Albina-art) |     [<img src="https://avatars2.githubusercontent.com/u/7222512?v=4&s=460" width="100px;"/><br /><sub>maniack</sub>](https://github.com/maniack)<br />     |
|  [<img src="https://avatars2.githubusercontent.com/u/18503575?v=4&s=460" width="100px;"/><br /><sub>hadidimad</sub>](https://github.com/hadidimad)   | [<img src="https://avatars0.githubusercontent.com/u/12181586?v=4&s=460" width="100px;"/><br /><sub>GhostRussia</sub>](https://github.com/GhostRussia)  | [<img src="https://avatars3.githubusercontent.com/u/608906?v=4&s=460" width="100px;"/><br /><sub>sourcesoft</sub>](https://github.com/sourcesoft) |    [<img src="https://avatars2.githubusercontent.com/u/10848952?v=4&s=460" width="100px;"/><br /><sub>zhuharev</sub>](https://github.com/zhuharev)    | [<img src="https://avatars0.githubusercontent.com/u/3918844?s=460&v=4" width="100px;"/><br /><sub>nuxdie</sub>](https://github.com/nuxdie)  |  [<img src="https://avatars0.githubusercontent.com/u/1156226?s=460&v=4" width="100px;"/><br /><sub>Seklfreak</sub>](https://github.com/Seklfreak)   |

## Donate

Bitcoin : `1KjcfrBPJtM4MfBSGTqpC6RcoEW1KBh15X`

[![Analytics](https://ga-beacon.appspot.com/UA-107698067-1/readme-page)](https://github.com/igrigorik/ga-beacon)
