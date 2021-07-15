# What is BootStrap?
- Responsive front-end library

# Try this:
- Button from "cssbuttongenerator.com"
- in Codeply add a button with the following classes:
    - "btn btn-primary"
    - "btn btn-dark"
- in Codeply add a DIV as below:
```html
<div class="jumbotran">
Hello World
</div>
```

# Installing Bootstrap
Start by creating a new file `index.html`.
Get the download links for Bootstrap from `www.getbootstrap.com`
```html
<html>
    <head>
        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
    </head>
</html>
```
CDN: Content Delivery Network
Interesting link: `www.submarinecablemap.com`

Try adding a new header tab to the above HTML
```html
<body>
<h1>Hello World</h1>
</body>
```
Easiest way to get started with using Bootstrap is through starter template [here](https://getbootstrap.com/docs/5.0/getting-started/introduction/#starter-template)

Third way of installing Bootstrap is to download the library from the Bootstrap website.
- This is not a recommended way as the browser has to download all of the library files.


# Web Design 101 - Wireframing
- Wireframing - Low fidelity representation of a website
- Mockup - High fidelity representation of a website

Try this: `ui-patterns.com` and `dribble.com`.

Let's start by creating a wireframe (using a pencil-and-paper)
- Sneakpeekit
- Balsamiq.cloud

Create a wireframe in Balsamiq (create a new account) and create a new project.

# Bootstrap Navigation Bar
Let's starting a navigation bar.

```html
<nav>
    <ul>
        <li>Contact</li>
    </ul>
</nav>
```
Add the following class to the `nav` above:
- navbar

Add the following classes to `ui`
- navbar-nav

And add the following class to `li`
- nav-item

Change the content "Contact" to an anchorage
```html
<a class="nav-link" href="">Contact</a>
```

Add the following additional navbar items:

```html
<nav class="navbar">
    <ul class="navbar-nav">
        <li class="nav-item">
            <a class="nav-link" href="">Contact</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Pricing</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Download</a>
        </li>
    </ul>
</nav>
```

The above items will be stacked vertically. To stack them horizontally add the class `navbar-expand-lg` to the `nav` tag above.

Add a style or background to the navbar using the class `bg-lignt`

We can also change the text color using `navbar-lignt` or `navbar-dark`.

We can add a brand using the following:
```html
<nav class="navbar">
    <a class="navbar-brand" href="">BrandName</a>
    <ul class="navbar-nav">
        <li class="nav-item">
            <a class="nav-link" href="">Contact</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Pricing</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Download</a>
        </li>
    </ul>
</nav>
```

How to shift all of the links to the left?

Apply the following class to the `ul` tag
- ml-auto

When resizing the browser, the above navbar changes to a vertical stack. We can change this behavior to display a drop-down instead.
Steps:
- Add the following button inside the `nav`.
```html
 <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
```

- Enclose brand and `ul` in a div:
```html
<div class="collapse navbar-collapse" id="navbarSupportedContent">
    <a class="navbar-brand" href="">BrandName</a>
    <ul class="navbar-nav">
        <li class="nav-item">
            <a class="nav-link" href="">Contact</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Pricing</a>
        </li>
        <li class="nav-item">
            <a class="nav-link" href="">Download</a>
        </li>
    </ul>
</div>
```

# Bootstrap Grid Layout System
Add the following code:
```html
<div class="row">
    <div class="col" style="background-color:red; border: 1px solid;">
        col
    </div>
</div>
```
This occupies 100% of the screen width. Adding more `div` tags takes up proportion of the screen.
```html
<div class="row">
    <div class="col" style="background-color:red; border: 1px solid;">
        col
    </div>
        <div class="col" style="background-color:red; border: 1px solid;">
        col
    </div>
    <div class="col" style="background-color:red; border: 1px solid;">
        col
    </div>

</div>
```

In Bootstrap we can specify the number of columns the `div` element should take using a number after the class `col` for example, `col-6` will take 6 columns.

The total for a single-row is 12. That means `col-3` will only take up a quarter of the screen.


