# Boilerplate Bootstrap Vanilla
Simple boilerplate project to get started with Bootstrap.

By Vanilla I mean this is basic html/css/javascript, without requiring any build steps to run the project.


## Explanations

```html
<html lang="en">
```
Update the `lang` attribute on the `html` tag, to match the content language.

`en` for English, and `da` for Danish.

Here is a list of language codes: https://gist.github.com/JamieMason/3748498

---

```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```
This viewpoint meta tag, helps the site scale as expected on all devices.

---

```html
<script src="js/script.js" defer></script>
```
If scripts are included in the `head`, make sure to add `defer` to let the DOM
finish loading before running the javascript.

Inline scripts (`<script></script>`), can not be deferred. So that needs to be
placed at the end of the `body` tag.

---

```html
<body class="min-vh-100 overflow-y-scroll d-flex flex-column">
```
- `min-vh-100`: Make sure the body can not get smaller than filling the screen height.
- `overflow-y-scroll`: Make sure the scrollbar is always visible, to avoid the content jumping when it show up.
- `d-flex flex-column`: Make the whole page use flexbox, in the column direction. Makes `nav`, `main` and `footer` stack vertically.

---

```html
<main class="flex-grow-1">
```
- `flex-grow-1`: Let the main content grow to fit the minimum height of the parent flexbox.

---

## Quick start

### Header

Default content of the header section.
```html
<header>
    <!-- Your navigation could live here, or you can delete the header tag -->
</header>
```

---

Basic navbar, you can insert in the `header` tag.
This is set to dark mode, you can use light mode by removing `data-bs-theme="dark"`.
```html
<nav class="navbar navbar-expand-lg bg-body-tertiary" data-bs-theme="dark">
    <div class="container-fluid">
        <a
            class="navbar-brand"
            href="#"
        >
            Template
        </a>
        <button
            class="navbar-toggler"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#navbarNav"
            aria-controls="navbarNav"
            aria-expanded="false"
            aria-label="Toggle navigation"
        >
            <span class="navbar-toggler-icon"></span>
        </button>
        <div
            id="navbarNav"
            class="collapse navbar-collapse"
        >
            <ul class="navbar-nav">
                <li class="nav-item">
                    <a
                        class="nav-link active"
                        href="#"
                        aria-current="page"
                    >
                        Home
                    </a>
                </li>
                <li class="nav-item">
                    <a
                        class="nav-link"
                        href="#"
                    >
                        Features
                    </a>
                </li>
                <li class="nav-item">
                    <a
                        class="nav-link"
                        href="#"
                    >
                        Pricing
                    </a>
                </li>
                <li class="nav-item">
                    <a
                        class="nav-link"
                        href="#"
                    >
                        About us
                    </a>
                </li>
            </ul>
        </div>
    </div>
</nav>
```

### Main

Default content of the main section.
```html
<main class="flex-grow-1">
    <section class="container mt-4">
        <h1>Bootstrap Template Vanilla</h1>
        <p>
            This is a template to getting started building a webapp using Bootstrap.
        </p>
    </section>
</main>
```

---

Starting point for having a large hero section at the start of the page.
```html
<main class="flex-grow-1">
    <section
        class="ratio ratio-16x9"
        style="
            background-image: url('https://picsum.photos/1920/1080/?grayscale&blur=4');
            background-size: cover;
            background-position: center;
        "
    >
        <div class="p-5 text-white">
            <h1 class="display-1">Welcome</h1>
            <div class="display-5">
                You can have a pretty header here
            </div>
        </div>
    </section>
    <section class="container mt-4">
        <h1>Bootstrap Template Vanilla</h1>
        <p>
            This is a template to getting started building a webapp using Bootstrap.
        </p>
    </section>
</main>
```
