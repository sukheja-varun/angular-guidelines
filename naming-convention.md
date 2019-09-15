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
1. Use **camelCase** when naming variables for objects, functions, and instances.
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
    
1. Variables for service instance should be prefixed with underscore ( _ ) and shouldn't contain keyword service as suffix.    
    ```
    // bad
    private toast:ToastService  // _ not prefixed
    private loaderService:LoaderService    // service as suffix not to be used
    
    // good
    private _toast:ToastService
    ```
1. Variables for http service instance should be prefixed with underscore ( _ ) and use Http as suffix.    
    ```
    // bad
    private _customerHttp:CustomerReviewHttpService  // _ not prefixed
    private _loader:LoaderService   // not used Http as suffix
    private loaderService:LoaderService    // instad of Http as suffix, Service is used
    
    // good
    private _customerHttp:CustomerReviewHttpService
    ```
1.  Use suffix as **List** for variables of data type - Array, eg customReviewList
1.  Use suffix as **Set** for variables of data type - Set, eg customReviewSet
1.  Use suffix as **Map** for variables of data type - Map, eg customReviewMap

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
    
## Enums
1. Use ProperCase (PascalCase) when naming enums and all the keys should be UPPER_CASE.
    ```
    // bad
    enum myDirection {
        up,
        right,
        down,
        left
    }
    
    // good
    enum MyDirections {
        UP,
        RIGHT,
        DOWN,
        LEFT
    }
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
1. Use UPPER_CASE naming for **readonly** class properties.
    

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
    
