## General (applied to all)

1. Avoid single letter names. Be descriptive with your naming.
    ```
    // bad
    function q() {
      // ...
    }

    // good
    function query() {
      // ...
    }
    ```
    
    
## Variables

1. Use **camelCase** when naming variables for objects, functions, and instances
    ```
    // bad
    let OBJEcttsssss = {};
    let this_is_my_object = {};
    let c = function() {}

    // good
    let thisIsMyObject = {};
    let thisIsMyFunction = function() {}
    ```

1. Use **let** instead of var for declaring variables.
    ```
      // bad 
      var myName = 'Varun Sukheja';
      
      // good
      let myName = 'Varun Sukheja';
    ```
    
## Constants
1. User **UPPER_CASE** when naming constants and use underscore(_) as seperator.
    ```
    // bad
    export const THING_TO_BE_CHANGED = 'should obviously not be uppercased';

    // bad
    export let REASSIGNABLE_VARIABLE = 'do not use let with uppercase variables';

    // ------------------------------------

    // bad
    export const apiKey = 'SOMEKEY';
        
    // good
    export const API_KEY = 'SOMEKEY';
    
    // ------------------------------------
    
    // bad - no need to uppercases objec key, only uppercase object name
    export const MAPPING = {
      KEY: 'value'
    };
    
    // good
    export const MAPPING = {
      key: 'value'
    };    
    ```

## Classes
1. Use ProperCase (PascalCase) when naming classes (service, component, module, etc).
    ```
    // bad
    class user {
      constructor(options) {
        this.name = options.name;
      }
    }

    const bad = new user({
      name: 'nope',
    });
    
    // good
    class User {
      constructor(options) {
        this.name = options.name;
      }
    }

    const good = new User({
      name: 'yup',
    });
   ``` 

## Interfaces

1. Use ProperCase (PascalCase) when naming interfaces.
    ```
    // bad
    interface person {
      name: string;
      age:  number;
    }  
    
    // good
    interface Person {
      name: string;
      age:  number;
    }  
    ```
    
## Folders
1. Use **lower-case** when naming folders and use hypehn(-) as seperator.
    ```
    // bad 
    laguageTranslation
    LaguageTranslation
    Laguage-Translation
    
    // good
    laguage-translation (using - as seperator)
    ```

## Files
1. File naming pattern should be `<file-name>.<file-type>.<extension>`.

    File type could be model, constant, module, component, directive, guard, interceptor, service, etc.
    ```
    // bad
    sidebarMenu.constant.ts // file name should not be in camelCase
    NotFound.component.ts // UpperCase name not allowed
    api.ts  // file type is missing
    
    // good
    sidebar-menu.constant.ts
    not-found.component.ts    
    ```

1. Use **lower-case** when naming folders and use hypehn(-) as seperator.
    ```
    // bad 
    laguageTranslation
    LaguageTranslation
    Laguage-Translation
    
    // good
    laguage-translation // using - as seperator
    
