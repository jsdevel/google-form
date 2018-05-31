# google-form [![NPM version][npm-image]][npm-url] [![Downloads][downloads-image]][npm-url]
> Simple AJAX request to POST data to a google form.

## How to use

* Create a form in google drive.

![Creating a form](./images/create-google-form.png)

* Copy the form URL up to `/edit`.

![Copy form URL](./images/new-form.png)

* Use the URL as the `action` attribute of your `form` in HTML:

```html
<form method="POST"
      action="https://docs.google.com/forms/d/1gci224y12YpOnxudXm_wUIM1da474gI6pE9AborYAew"
      onsubmit="return window.submitGoogleForm(this);">

  <label>name</label>
  <!-- view the form and inspect inputs to get the generated names. -->
  <input name="entry.2345234">

  <button type=submit>Submit</button>
</form>
```

* Load `./google-form.js` in your browser, or `require` it with browserify or webpack.
* That's it!

## LICENSE
``````
The MIT License (MIT)

Copyright (c) 2015 Joseph Spencer

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
``````

[downloads-image]: http://img.shields.io/npm/dm/google-form.svg
[npm-url]: https://npmjs.org/package/google-form
[npm-image]: http://img.shields.io/npm/v/google-form.svg
