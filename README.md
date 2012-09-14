-O_o- eXtension Functionality Aspect
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

<i><b>Add binding event for ASPECT already create variable</b></i>
```javascript
 foo.name_of_property.__aspect__.__before__ = { 
      get: function(current) { /* todo code here */ },
      set: function(current, settable) { /* todo code here */ }
 }
```

<i><b>Get all binding event for ASPECT already create variable</b></i>
```javascript
 console.log(foo.name_of_property.__aspect__.__before__) // [ { get: /**/, set: /**/ } ]
```


<i><b>Delete ALL binded event for ASPECT already created variable</b></i>
```javascript
 foo.name_of_property.__aspect__ = [undefined]
```

Howto to work library?
===========
<pre>


</pre>

Howto to work library?
===========
Double License
1) EULA (for commercial usage, upon request)
2) Creative Commons 3.0 Attribution - No-Commercial (BY-NC)