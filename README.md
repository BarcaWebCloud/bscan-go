## bscan-go 0.1.0

### Get the bscan-go module

Note that you need to include the **v** in the version tag.

```sh
go get github.com/BarcaWebCloud/bscan-go@v0.1.0
```

A Go library for scan any computational device and atmospheric environment.

Requeriments:

* [GO lang](https://go.dev/doc/install)



### Tests

We will start a series of tests of our `golang package`.
By default Go comes with rudimentary test capabilities that looks for files ending with **_test.go**.

<br>

Run the tests using the following command:

```
go test
```

<br>

If everything passed, tidy up a bit by running:

```
go mod tidy
```

Then run the tests again, just to be sure:

```
go test
```

For more verbose output try this:

```
go test -v
```

Sometimes test results are cached. To make sure they are not, use this command:

```
go test -count 1
go test -v -count 1
```

For more information on testing, run this command:

```
go help testflag
```