# sdc
![Version](https://img.shields.io/badge/version-v1.0-blue)
![License](https://img.shields.io/badge/license-GPLv3-orange)

`sdc` (**seek docker-compose**) is a utility for finding and elegantly running `docker-compose` of desired images. It allows for displaying of all directories below `~` that include a `docker-compose` file, choosing the wanted end directory, and automatically running `docker-compose up -d` in it.

## Usage
`sdc` should be executable and preferably put into the `~/bin` directory, which is included in `$PATH` on default.

## Run
We run the executable as `source`
```sh
chmod +x sdc

. sdc
```

## Alias
For convenience of not having to manually `source` through `.` every time, we can add an alias to `~/.bashrc`
```sh
alias sdc=". sdc"
```

Then, we can run the executable as
```sh
sdc
```

## Down
After choosing the end directory during program execution, we `cd` into it, effectively allowing us to close down the container whenever wanted through
```sh
docker-compose down
```
