google-form-styling
===================

A stylesheet to be used if you want to create your own theme for a Google form. The stylesheet is written with [LESS](http://lesscss.org) so that it is easy to customize.

### Demo

[Demo form in action](https://googledrive.com/host/0B3SHb_huRFdyNENfQjVzSGpIOFU/index.html)

### Stylesheet content

As a starting point I basically just copied the stylesheet from the default Google form page. Then I took all the colors and placed them into variables. The stylesheet needs to be stripped of things not necessary.

### Moving Forward

I do not want to add any extra markup to the pages. The idea hear is to just copy the form mark that Google gives you and then just add a stylesheet that will make it themed.

*Think themes for bootstrap. Markup stays, stylesheets change.*

But right now I am just going to try and normalize the current stylsheet into something as default as possible so that I can then create a my-theme-name.css file that contains all the variables to do the styling. I am currently only using the variables in LESS but eventually I will use more of the feaures to get everything nice and themeable.

### How to create a custom form

* Create a form as normal
* Click the view live form
* Copy everything inside the form tag including the form tag itself
* Create a new blank HTML file
* Create an empty div with a `container` class
* Paste all the form markup inside there
* Link the style.css stylsheet
* Test the form and check the response in Google drive

### Hosting the form

Something relatively new to Google drive is the ability to host static HTML pages.

* Create a public shared folder
* Upload all your **static** html files
* Open the `index.html` file in drive and click the **preview button**
* Copy the link to the page it sends you too
* Share that link with whoever because you are done!

This is how the [demo form](https://googledrive.com/host/0B3SHb_huRFdyNENfQjVzSGpIOFU/index.html) is hosted.

### lesswatch.js

just run `node lesswatch css` and it will watch all .less files and compile them for you. The lesswatch is written by [idris](https://gist.github.com/idris/1080416).

### I am a LESS hater and I <3 SASS/STYLUS/BABIES

Well then find and replace all `@varName` signs with `$varName` or just make the variables `varName = value` for Stylus.

I picked LESS because it has a lower barrier to entry than SASS or STYLUS. Even though I <3 Stylus the best.


### License

(The MIT License)

Copyright (c) 2013 James Doyle([@james2doyle](http://twitter.com/james2doyle)) james2doyle@gmail.com

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
