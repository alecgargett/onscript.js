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

**Toggle**

```html
<button onclick='toggle_class(".dark")'>
Click Me
</button>
```

or

```html
<button onclick='toggle_class(".dark on this")'>
Click to toggle
</button>
```

or to target a specific element by ID

```html
<button onmouseover='toggle_class(".light on #div_id")'>
Hover to toggle
</button>
```

**GET request**

```html
<button onkeypress='get("/fragment")'>
Press any key to get fragment
</button>
```

or

```html
<button onkeypress='get("/fragment into this")'>
Press any key to get fragment
</button>
```

or to target the innerHTML of another div:

```html
<button onmousedown='get("/fragment into #div_id")'>
Click me to get fragment
</button>
```

or to target the outerHTML of another div:

```html
<button onclick='get("/fragment to replace #div_id")'>
Click me to get fragment 
</button>
```

**POST request**

```html
<div onload='post("/list")'>
Post on load
</div>
```

License: ag-copyleft (Free to use and modify on conditions of fair attribution, fair compensation, same license, and no liability for the copyright holder; no warranty)
