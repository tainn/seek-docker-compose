# seek-docker-compose
Seek docker-compose (`sdc`) is a utility for finding and elegantly running `docker-compose` of desired images. It allows for displaying of all directories below `~` that include a `docker-compose` file, choosing the wanted end directory, and automatically running `docker-compose up -d` in it.

## Usage
`sdc` should be executable and preferably put into the `~/bin` directory, which is included in `$PATH` on default.

We run the executable as `source`
```sh
. sdc
```

## Down
After choosing the end directory during program execution, we `cd` into it, effectively allowing us to close down the container whenever wanted through
```sh
docker-compose down
```
