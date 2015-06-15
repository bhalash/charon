# scss-helpers
These files are a small set of helper functions, mixins and partials that I reuse across projects. Becasue I work on proprietary projects I chose to use the MIT License instead of the GPL in order to sidestep any headaches about needing to open code. 

## Files

### \_media.scss
A responsive media query framework

### \_mixins.scss
File contains a combination of useful mixins and functions for use in Scss projects:

##### @position
Quickly set absolute, relative and fixed positions for elements, along with offsets. Three mixins serve as wrappers for @position:

    * @absolute
    * @fixed
    * @relative

##### @palette
Return the specified from your theme's palette of colours.

#### @prefix, @prefix-value
Add arbitrary vendor prefixes to properties and values.

#### @generate-social-link
Generate dynamically-resizable social media icons from the supplied vector stylesheets. Both white icons and black icons are available to use.

#### @cntent-padding
Set side padding for the main content based on the contents of a mapof @media breakpoints.

#### @flex-parent, @flex-child
Generate [flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) CSS rules for both parent and child flex elements, along with necessary vendor prefixes.

#### @square-flex
Generate square (or any aspect ratio) boxes using percentage sizes alone.

#### @vertical-center
Wrap element with equal padding above and below.

#### @rgba-opposite
Invert RGBA values.

#### @placeholder-styles
Style input placeholder text.

#### @solid-mask, @gradient-mask 
Extends %background-mask. Put a coloured mask behind an elements content.

#### @font-face
Generate CSS @font-face rules in a neat manner using a map.


### \_decimal.scss
Decial 

### \_partials.scss
A collection of miscellaneous Scss partials derived from mixins and functions in [\_decimal.scss](/_decimal.scss) and [\_mixins.scss](/_mixins.scss).

## License and Copyright
The MIT License (MIT)

Copyright (c) 2015 Mark Grealish

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

## Credit
Some mixins were derived from examples and concepts already present on the Internet, so I cannot make any claim to being an original creator. Something something truer to say that I stand upon the shoulder of giants.
