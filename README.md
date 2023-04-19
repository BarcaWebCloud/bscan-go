## BSCAN-GO 0.1.0

<br>

**BSCAN-GO** is a golang package made for Developers, Forensics Analysts, Infrastructure Engineers, Network Administrators and Entrepreneurs to use to obtain information and monitoring about certain computing devices. You can use your creativity to solve problems across mobile and web apps using **bscan-go**. 
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