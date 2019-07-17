The following functions help with diagnosing bugs and ensuring the correct state of variables and boolean tests.

## Panic

Force runtime errors with `panic()`. 

Use `panic` for unrecoverable states. It terminates the progam immediately and provides optional feedback. 

For example:

``` c++
function main()

    var x = 1;
    var y = 2;
    var z = y + x;
    printLn(toString(z));
    z =- 2;
    if (z != -1)
    	panic("This is a terrible mistake!");
    endif
    printLn(toString(z));

endfunction
```

## Assert

Use `assert` to ensure state.

For example:

``` c++
function main()

    var x = 1;
    var y = 2;
    var z = y + x;
    printLn(toString(z));
    z =- 2;

    assert(z == 1);
    assert(z == 1, "khjkh")

    printLn(toString(z));

endfunction
```


<br/>