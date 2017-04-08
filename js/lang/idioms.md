Like all languages, idiom exists and people like it. This documents will archive all the idioms I met.

#### Type Conversion idiom

```javascript
x + ""    // Same as String(x)
+x        // Same as Number(x), you may also see x-0
!!x       // Same as Boolean(x), Note double !
```

### `||` operator idiom

```javascript
// if max_width is defined, use that,
// Otherwise look for a value in the `preferences` object,
// If that is not defined use a hard-coded constant.
var max = max_width || preferences.max_width || 500;

// supply default values for parameters.
function copy(o, p) {
  p = p || {}; // if no object passed for p, use a newly created object.

  // function body goes here
}
```
