Travis-CI Build Status: [![Build Status](https://app.travis-ci.com/mrckurz/go-mux.svg?branch=master)](https://app.travis-ci.com/github/mrckurz/go-mux)

# go-mux: Microservice in GoTutorial

- Tutorial from [semaphoreci.com](https://semaphoreci.com/community/tutorials/building-and-testing-a-rest-api-in-go-with-gorilla-mux-and-postgresql)

## Prerequisites:
1. [GitHub Account](https://github.com)
2. PostgreSql installed and configured ([see Tutorial](https://www.codementor.io/@engineerapart/getting-started-with-postgresql-on-mac-osx-are8jcopb))
  * make sure user/role 'postgres' is available
  * environment variables properly set
     * export APP\_DB_USERNAME=postgres
	  * export APP\_DB_PASSWORD=\postgres
	 * export APP\_DB_NAME=postgres
3. GoLang installed (see [golang.org](https://golang.org))


## Run the Project in CMD
1. Tests DB: docker run -p 5432:5432 --name some-postgres -e POSTGRES_PASSWORD=postgres -d postgres
2. UnitTests: go test -v


### Hints/Info
- When you run go test it compiles all the files ending in _test.go into a test binary and then runs that binary to execute the tests. Since the go test binary is simply a compiled go program, it can process command line arguments like any other program 
- 2nd part: add Travis (.travis.yml), see [docs.travis-ci.com](https://docs.travis-ci.com/user/tutorial/#to-get-started-with-travis-ci)