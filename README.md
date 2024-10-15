# onscript.js

OnScript.js is a project with the goal of creating a minimalist vanilla javascript library of functions with natural language arguments.

There are three primary design goals:

* Functionality: to eventually include all of the functionality of htmx, hyperscript, datastar, unpoly, Alpine AJAX, Hotwire, Liveview, Livewire, Hydro, JQuery etc.
* Syntax: to use a combination of vanillaJS event handler function calls with syntax inspired by hyperscript/Hypertalk/Lua/JQuery.
* Spec: to remain in spec and use "on*" inline event listeners where feasible.

which aim to serve three primary user exeprience goals:

* Simplicity of development
* Code readability and maintainability
* Power and flexibility in website application design
* Fast and efficient application performance

OnScript in practice will look like:

*Toggle*

```html
<button onclick='toggle_class(".red")'>
Click Me
</button>
```

```html
<button onclick='toggle_class(".toggled_class" on "#div_id")'>
Click Me
</button>
```

*GET request*

```html
<button onclick='get("/example")'>
Click Me
</button>
```

or to target the innerHTML of another div:

```html
<button onclick='get("/example" into "#div_id")">
Click Me
</button>
```

or to target the outerHTML of another div:

```html
<button onclick='get("/example" to_replace "#div_id")">
Click Me
</button>
```

*POST request*

```html
<button onclick='post("/test")'>
Click Me
</button>
```

Copyright Alec Gargett 2024

License: ag-copyleft
