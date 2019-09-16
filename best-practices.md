## `null` and `undefined`
Use undefined. Do not use null.


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
