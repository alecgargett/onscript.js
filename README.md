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

```html
<button onmouseover='toggle_class(".light on #div_id")'>
Click Me
</button>
```

**GET request**

```html
<button onkeypress='get("/fragment")'>
Click Me
</button>
```

or to target the innerHTML of another div:

```html
<button onmousedown='get("/fragment into #div_id")'>
Click Me
</button>
```

or to target the outerHTML of another div:

```html
<button onclick='get("/fragment to_replace #div_id")'>
Click Me
</button>
```

**POST request**

```html
<button onload='post("/list")'>
Click Me
</button>
```

2024

License: ag-copyleft (Free to use and modify on conditions of fair attribution, fair compensation, same license, and no liability for the copyright holder; no warranty)
