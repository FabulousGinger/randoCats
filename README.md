# RandoCats!

----
## What is RandoCats?

>RandoCats will query the Giphy API to serve the GIF using GO.


----
## Setup

* Download and install [GO](https://golang.org/dl/)!
* If using the Dockerfile, Download and install [Docker](https://www.docker.com/products/docker-desktop)
* Copy the `cmd/example.env` to `cmd/.env`
* Enter an Giphy API key. To get an API key, create an app from [Giphy](https://developers.giphy.com/dashboard/)

----
## How To Use

* RandoCats work by passing os arguments, where ratings is optional(g, pg, pg-13, r):
`go run main.go [APIKEY] [TAG] [RATING]`
* The API key can be stored in a `cmd/.env` file instead of passing it through the command line.

* Run manually by running main.go inside the `cmd/` dir.
`go run main.go cat`

* To use Docker build and run from the Dockerfile.
`docker build -t randocats .`
`docker run -d -p 8080:8080 --name randocats roandocats`

* RandoCats will be served on port `8080`

----
## Authors

* **James von Hagel**
[FabulousGinger](https://github.com/FabulousGinger)
