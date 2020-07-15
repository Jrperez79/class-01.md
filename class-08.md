# Class-08 Reading

## Local Storage
The Past, Present and Future of Local Storage for Web Apps

### Diving In
Persistent local storage is one of the areas where native client applications have held an advantage over web applications.  

These values may be stored in the registry, INI files, XML files, or some other place according to platform convention.

Cookies
Cookies are used for persistent storage of small amounts of data. But they have 3 potential dealbreaking down sides:
    - Cookie are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
    - Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web app is served over SSL).
    - Cookies are limited to about 4KB of data -- enough to slow down your application, but not enough to be terribly useful.

What we really want is...
    - a lot of storage space
    - on the client
    - that persists beyond a page refresh
    - and isn't transmitted to the server

Before HTML5, all attempts to achieve this were ultimately unsatisfactory in different ways.

### History of Local Storage

userData
    - Allows web pagers to store up to 64K of data per domain, in a hierarchical XML-based structure.  (Trusted domains, such as intranet sites, can store 10 times that amount.).

### HTML5 Storage
HTML5 is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons.  Certain browsers vendors also refer to it as Local Storage or DOM storage.

What is HTML5 storage?
Simply put, it's a way for a web page to store named key/value pairs locally, within the client web browser

### Using HTML5 Storage
Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key.

If you are storing anything other than strings, a function like parseInt() or parseFloat() can retrieve data into the expected JS datatype.

Calling setItem() with a named key that already exists will silently overwrite the previous value.

Calling getItem() with a non-existent key will return null rather than throw an exception.

You can treat the localStorage object as an associative array.  
Ex: localStorage.getItem() -> localStorage.setItem or var foo = localStorage["bar"]; -> localStorage["bar"] = foo;

There are also methods for removing the value for given named key, and clearing the entire storage area (deletes all the keys and values at once.)
Ex: interface Storage { deleter void removeItem(in DOMString key); void clear();};

### Tracking Changes To The HTML5 Storage Area
The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called.

### Limits in Current Browsers
5 megabytes is how much storage space each origin gets by default.

"QUOTA_EXCEEDED_ERR" is the exception that will get thrown if you exceed your storage quota of 5mb.  No you cannot use more storage space.

### HTML5 Storage In Action
With HTML5 we can save the progress locally, within the browser itself.







