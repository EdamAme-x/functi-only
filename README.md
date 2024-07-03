# functi-only
Functi is Function-only Porgramming Language  
This is joke, but it's not joke.  

By enclosing a module by module name, the module can be used in a process within its arguments.  
Scope is valid only within the argument.

## procedure
```javascript
(
  imports(
    std,
    math
  ),
  std(
    define(a, int(5)),
    define(b, nil()),
    math(
      assign(b, randomInt(int(0), int(10)))
    ),
    if(
      equal(
        a,
        b
      ),
      print(b, string(is 5)),
      print(b, string(is not 5)
    )
  )
)
```

## module
```javascript
(
  imports(
    std,
    math
  ),
  std(
    defineFunction(isDiv3,
      defineArgs(num),
      math(
        if(
          equal(mod(num, int(3)), int(0)),
          return(true()),
          return(false())
        )
      )
    ),
    exports(
      isDiv3
    )
  )
)
```
