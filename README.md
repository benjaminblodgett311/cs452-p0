# Greeting Message
## CS452 Project 0

- Name: Benjamin Blodgett
- Email: benjaminblodgett311@u.boisestate.edu
- Class: 452-002

## Experience

This project was really easy. I was curious how you could get 100% code coverage so I tried dereferencing a malloc'd pointer in the branch where it returns null. I realized that this block was ommited from testing. I added a bit to this README.md for using live-serever because I think it's more convenient when the coverage files change rather than constantly reopening them in the browser.

## Makefile

To build the project run:

```bash
make release
```
To run the executable:

```bash
./build/release/myapp
```

To run the unit tests:

```bash
make test && make check
```

To see all the configurations, run `make help`

```bash
Usage: make [target]
Available targets:
  debug     - Build the application in debug mode (default)
  release   - Build the application in release mode
  test      - Build the unit tests
  all       - Builds debug, release, and test targets
  check     - Run tests and check results
  report    - Generate coverage report after running tests
  leak      - Check for memory leaks in debug mode
  clean     - Remove build artifacts
  print     - Print build variables for MakeFile debugging
  help      - Show this help message
```

Report watching (run after unit tests):

```bash
make report
cd build/report/html
live-server . watch=*.html
```
