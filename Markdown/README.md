# Markdown

    Markdown Cheatsheet.

# Table of Contents

- [Markdown](#markdown)
- [Table of Contents](#table-of-contents)
- [Images](#images)
- [Custom Style](#custom-style)
  - [Custom Tags](#custom-tags)
  - [Overwriting Tags](#overwriting-tags)

# Images

```html
<p align="center" width="100%">
    <img src="path">
</p>
```

# Custom Style

## Custom Tags

```html
<style>
  r { color: Red }
</style>
```

## Overwriting Tags

```html
<!-- Removing Pre-Existing Styling -->
<style>
    s { text-decoration: none }   /* Strike-Through */
    em { font-style: normal }     /* Italic Emphasis */
</style>


<!-- Overwriting with Color Styling -->
<style>
    s { color: Seagreen }
    em { color: Red }
</style>
```
```html
<!-- Example -->
~~This will be Seagreen~~
 _This will be Red_
 ```