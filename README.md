CKEditor 5 classic editor build
========================================

[![npm version](https://badge.fury.io/js/%40ckeditor%2Fckeditor5-build-classic.svg)](https://www.npmjs.com/package/@ckeditor/ckeditor5-build-classic)
[![Coverage Status](https://coveralls.io/repos/github/ckeditor/ckeditor5/badge.svg?branch=master)](https://coveralls.io/github/ckeditor/ckeditor5?branch=master)
[![Build Status](https://travis-ci.com/ckeditor/ckeditor5.svg?branch=master)](https://travis-ci.com/ckeditor/ckeditor5)

The classic editor build for CKEditor 5. Read more about the [classic editor build](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/overview.html#classic-editor) and see the [demo](https://ckeditor.com/docs/ckeditor5/latest/examples/builds/classic-editor.html).

![CKEditor 5 classic editor build screenshot](https://c.cksource.com/a/1/img/npm/ckeditor5-build-classic.png)


## Quick start

First, install the build from npm:

```bash
npm install --save ckeditor5-disamina
```

And use it in your website:

```html
<div id="editor">
	<p>This is the editor content.</p>
</div>
<script src="./node_modules/ckeditor5-disamina/build/ckeditor.js"></script>
<script>
	ClassicEditor
		.create( document.querySelector( '#editor' ) )
		.then( editor => {
			window.editor = editor;
		} )
		.catch( error => {
			console.error( 'There was a problem initializing the editor.', error );
		} );
</script>
```

Or in your JavaScript application:

```js
import ClassicEditor from 'ckeditor5-disamina';

// Or using the CommonJS version:
// const ClassicEditor = require( 'ckeditor5-disamina' );

ClassicEditor
	.create( document.querySelector( '#editor' ) )
	.then( editor => {
		window.editor = editor;
	} )
	.catch( error => {
		console.error( 'There was a problem initializing the editor.', error );
	} );
```

**Note:** If you are planning to integrate CKEditor 5 deep into your application, it is actually more convenient and recommended to install and import the source modules directly (like it happens in `ckeditor.js`). Read more in the [Advanced setup guide](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/advanced-setup.html).
