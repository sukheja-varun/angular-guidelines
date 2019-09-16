# Documentation

Use below mentioned plugin for auto generating method docs
https://marketplace.visualstudio.com/items?itemName=joelday.docthis


Sample method documentation snippet
```
  /**
   * @description It is used to display error alert modal
   *
   * @param {string} [title='Error!!!'] header title to be displayed in Modal
   * @param {string} [body='Please try again']  message body to be displayed in Modal
   * @memberof ToastService
   * 
   * TODO: 
   * - add OkButtonText and cancelButtonText properties
   * - write meaningful title and body
   */
   error(title: string = 'Error!!!', body: string = 'Please try again') {}
```

## Method Documentaion

- @description : describes the functionality of the method.
- @param describes the arguments received by method. It also tells the data type and usage.
- @return describes the return param with it's data type and usage.
- @member describes the class to which the method belongs tol

## TODOs
- TODO is used for things to be done later, Use `TODO:` in comment section for defining TODO.
- FIX is used for things to be fixed later, Use `FIX:` in comment section.
- NOTE is used for to provide any extra info, Use `NOTE:` in comment section.
- OPTIMIZE is used to display if any optimization is needed, Use `OPTIMIZE:` in comment section
- HACK is used to describe any hack used, Use `HACK:` in comment section.
- Use @CRITICAL, @HIGH and @LOW to describe priority.

Use below mentiond vs-code plugins for better TODOs handling.
- https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight
- https://marketplace.visualstudio.com/items?itemName=fabiospampinato.vscode-todo-plus
