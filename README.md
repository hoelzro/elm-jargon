# Elm Jargon File

This is a repository for tracking the jargon used by the Elm community.

# Constructor

Used to indicate one of the "branches" of a data type.  For example, the
`Maybe` type looks like this:

```elm
type Maybe a = Just a | Nothing
```

`Just` and `Nothing` are *constructors* for the ''Maybe'' type.

Sometimes referred to as *tags*.

# Currying

A function is *curried* if it takes a single argument and returns another function.  For
example, a binary `add` function would take an argument, and return another function, which,
when given its own argument, would add it to the first argument and yield the result.  It
would look like this in JavaScript:

```javascript
function add(a) {
    return function(b) {
        return a + b;
    };
}
```

All Elm functions are curried.

# Tag

See also [Constructor](#constructor).

# TEA

[The Elm Architecture](http://guide.elm-lang.org/architecture/index.html)
