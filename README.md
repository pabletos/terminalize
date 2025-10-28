# terminalize
<p align="center">
  <img src="https://raw.githubusercontent.com/pabletos/terminalize/main/img/terminalize.svg" alt="Terminalize logo" width="250">
</p>
<p>
<a 
  href='https://github.com/pabletos/terminalize/releases/tag/1.0'
  target='_blank'
  rel="noreferrer"
>
  <img src='https://img.shields.io/badge/version-1.0-green?logo=github' border='0' alt='latest release' />
</a>
<a 
  href='https://ko-fi.com/B0B1PYK0W'
  target='_blank'
  rel="noreferrer"
>
  <img height='32' style={{border:'0px', height:'36px'}} src='https://storage.ko-fi.com/cdn/kofi2.png?v=3' border='0' alt='Buy Me a Coffee at ko-fi.com' />
</a>
</p>

Terminalize is <b>a simple and lightweight CSS3 micro-framework</b> for doing terminal-like interfaces. [You can check a live version with examples here](https://terminalize.pablohuet.com/)

## Motivation

Terminalize was, in his humble beginnings, an old personal website I did based on a old codepen.

The main purpose of that website, at that time, was only to show my former CSS and web development skills. So I also created a blog with curious posts about code and projects.

But as I discovered not so many time later, the big majority of devices screens at that time showed the website too blurry and out of focus. So I had to discard that design and create a new website from scratch.

Some time ago I re-discovered this project buried in my files and decided to transform it in a some kind of micro-css framework for quick terminal style alike websites.

## Features

* Default and alternate styles for most HTML tags
* Fully styled forms and form inputs including buttons and selects
* **NEW**: Customizable Select Elements (2025) - Modern styling with full control over dropdown appearance
* Responsive design using `.panel`, `.row` and `.col` classes
* Unique styled code blocks
* Optional animations, filters and much more to obtain a retro terminal style

## How To use it

I designed **Terminalize** to be used with any other framework or existing style, so you only need to put a class `.terminalize` in the parent to have all the children correctly styled. Then inside you have to use a first `div` element with a `.screen` class to correctly apply the theme background color.

## Select Elements

Terminalize supports both traditional and modern customizable select elements:

### Traditional Select (All Browsers)
```html
<div class="select">
    <select>
        <option value="">Choose option...</option>
        <option value="value1">Option 1</option>
        <option value="value2">Option 2</option>
    </select>
</div>
```

### Customizable Select (Chrome 130+, Edge 130+)
```html
<select class="customizable">
    <button>
        <selectedcontent></selectedcontent>
    </button>
    <option value="">Choose option...</option>
    <option value="value1">Option 1</option>
    <option value="value2">Option 2</option>
</select>
```

#### Customizable Select Classes:
- `.customizable` - Base class for new select styling
- `.compact` - Smaller padding and font size
- `.thick-border` - 2px border width
- `.rounded` - Rounded corners (optional for softer look)

#### Browser Support:
- ✅ Chrome 130+
- ✅ Edge 130+ 
- 🚧 Firefox (in development)
- 🚧 Safari (in development)

**Note**: Customizable selects provide progressive enhancement - they fall back gracefully to traditional styling in unsupported browsers while maintaining full functionality.
