# go-func-timer
golang function timer - taken from https://coderwall.com/p/cp5fya/measuring-execution-time-in-go


The author of that helpful article did not include a repo to pull it in as a package, which I felt
would be useful, so I created this, buf full credit goes to the original author.


## Example

Copied example:

```
func factorial(n *big.Int) (result *big.Int) {
    defer timeTrack(time.Now(), "factorial")
    // ... do some things, maybe even return under some condition
    return n
}
```

