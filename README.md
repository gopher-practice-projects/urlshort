# Exercise #2: URL Shortener

## Exercise details

The goal of this exercise is to create an [http.Handler](https://golang.org/pkg/net/http/#Handler) that will look at the path of any incoming web request and determine if it should redirect the user to a new page, much like URL shortener would.

For instance, if we have a redirect setup for `/docs` to `http://www.somesite.com/a-story-about-dogs` we would look for any incoming web request with the path `/dogs` and redirect them.

To complete this exercises you will need to implement the stubbed out methods in [handle.go](./handle.go). There are a good bit of comments explaning what each method should do, and there is also a [main/main.go](./mian/main.go) source file that uses the package to help you test you code and get an idea of what your program should be doing.

## Bonus

As a bonus exercises you can also...

1. Update the [main/main.go](./mian/main.go) source file to accept a YAML file as a flag and then load the YAML from a file rather than from a string.
2. Build a JSONHandler that serves the same purpose, but reads from JSON data.
3. Build a Handler that doesn't read from a map but instead reads from a database. Whether you use BlotDB, SQL, or something else is entirely up to you.