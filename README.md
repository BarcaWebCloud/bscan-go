## BSCAN-GO 0.1.0

<br>

[**BSCAN-GO**](https://pkg.go.dev/github.com/BarcaWebCloud/bscan-go) is a golang package made for Developers, Forensics Analysts, Infrastructure Engineers, Network Administrators and Entrepreneurs to use to obtain information and monitoring about certain computing devices. You can use your creativity to solve problems across mobile and web apps using **bscan-go**. 
<br>
With a plethora of capabilities in Scanning Hardware, Software and Atmospheric Systems.

<br>
<br>

### Get the bscan-go module

<br>

Note that you need to include the **v** in the version tag.

<br>

```sh
go get github.com/BarcaWebCloud/bscan-go@v0.1.0
```

<br>

A Go library for scan any computational device and atmospheric environment.

<br>

Requeriments:

* [GO lang](https://go.dev/doc/install)

<br>
<br>


## Publishing

Publishing steps
Use the following steps to publish a module.

Open a command prompt and change to your module’s root directory in the local repository.

Run go mod tidy, which removes any dependencies the module might have accumulated that are no longer necessary.

<br>

```
go mod tidy
```

<br>

Run `go test ./...` a final time to make sure everything is working.

This runs the unit tests you’ve written to use the Go testing framework.

<br>

```
go test ./...
```

ok      example.com/mymodule       0.015s
Tag the project with a new version number using the git tag command.

<br>

For the version number, use a number that signals to users the nature of changes in this release. For more, see Module version numbering.

<br>

```
git commit -m "mymodule: changes for v0.1.0"
git tag v0.1.0
```

<br>

Push the new tag to the origin repository.

<br>

```
git push origin v0.1.0
```

<br>

Make the module available by running the go list command to prompt **Go** to update its index of modules with information about the module you’re publishing.
Precede the command with a statement to set the `GOPROXY` environment variable to a **Go proxy**. This will ensure that your request reaches the *proxy*.

<br>

```
GOPROXY=proxy.golang.org go list -m github.com/BarcaWebCloud/bscan-go@v0.1.0
```

<br>

Developers interested in your module import a package from it and run the `go get` command just as they would with any other module. They can run the `go get` command for latest versions or they can specify a particular version, as in the following example:

<br>

```
go get github.com/BarcaWebCloud/bscan-go@v0.1.0
```

<br>
<br>

## Tests

We will start a series of tests of our `golang package`.
By default Go comes with rudimentary test capabilities that looks for files ending with **_test.go**.

<br>

Run the tests using the following command:

<br>


```
go test
```

<br>

If everything passed, tidy up a bit by running:

<br>

```
go mod tidy
```

Then run the tests again, just to be sure:

<br>

```
go test
```

For more verbose output try this:

<br>

```
go test -v
```

Sometimes test results are cached. To make sure they are not, use this command:

<br>

```
go test -count 1
go test -v -count 1
```

For more information on testing, run this command:

<br>

```
go help testflag
```

<br>
<br>

## Add Tags

To publish different versions of your package you need to tag it like this:

<br>

```
git tag v0.1.x
git push origin --tags
```
<br>

You need to update the tags after pushing or merging everything to the **main branch**.