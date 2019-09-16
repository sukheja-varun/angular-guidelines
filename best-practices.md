

## General
1. Use pure pipe if pipe gives same output each time on same input.
1. Use **canLoad** instead of canActivate if possible.
1. Use readOnly keyword for defining constant class properties.
1. Store API endpoints in a constant file under constants folder.
1. Error messages can be stored inside constant file.
1. Create custom types for better type checking functionality.
1. By default decalre class properties and methods as private untill needed outside of the class.
1. If a class is used only for type checking only then better to make it an interface instead.
1. Try to provide services at Root level which will make it a Singleton Service.
1. Put common components, pipes, directives in a Shared Module.
1. If shared module grows bigger, then try to split it into smaller multiple shared modules.
1. Make sure to unsubscribe any active subscriptions in the ngDestroy of each class.
1. Give documentation to each function containing business logic.


## `null` and `undefined`
Use undefined. Do not use null.


## References

1. Use `const` for all of your references; avoid using `var`.

    > Why? This ensures that you can’t reassign your references, which can lead to bugs and difficult to comprehend code.

    ```javascript
    // bad
    var a = 1;
    var b = 2;

    // good
    const a = 1;
    const b = 2;
    ```

1. If you must reassign references, use `let` instead of `var`.

    > Why? `let` is block-scoped rather than function-scoped like `var`.

    ```javascript
    // bad
    var count = 1;
    if (true) {
      count += 1;
    }

    // good, use the let.
    let count = 1;
    if (true) {
      count += 1;
    }
    ```

1. Note that both `let` and `const` are block-scoped.

    ```javascript
    // const and let only exist in the blocks they are defined in.
    {
      let a = 1;
      const b = 1;
    }
    console.log(a); // ReferenceError
    console.log(b); // ReferenceError
    ```
