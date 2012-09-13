-O_o- JavaScript eXtension Aspect
===========

***Annotation***

Extending methods

<i><b>Create new ASPECT variable for property</b></i>
```javascript
 foo = {};
 foo.__aspect__ = "name_of_property";
 foo.name_of_property = "Hello world";
 console.log(foo.name_of_property) // display "Hello world!"
```

<i><b>Delete ASPECT variable from property</b></i>
```javascript
 foo.__aspect__ = ["name_of_property", undefined];
```

<i><b>Binding event for ASPECT already create variable</b></i>
```javascript
 foo.name_of_property.__aspect__ = { 
    before: { 
      get: function(current) { /* todo code here */ },
      set: function(current, settable) { /* todo code here */ }
    },
    after: { 
      get: function(current) { /* todo code here */ }, 
      set: function(current, settable) { /* todo code here */ }
    }
 }
```

<i><b>Delete ALL binded event for ASPECT already created variable</b></i>
```javascript
 foo.name_of_property.__aspect__ = [undefined]
```