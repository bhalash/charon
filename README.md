# Charon
Charon<sup>[1](#footnote-1)</sup> is a programmatic [Scss][1] library designed to give control of CSS back to individual developers. Too many Sass libraries lock you in to a their developer's preferred design paradigm-they give you pregenerated CSS or only a limited set of mixins.

Charon intends to be the counterpoint library that grants flexible, descriptive tools to developers interested in a programmatic approach to their CSS. Some features include:

* Programmatic symmetric and asymmetric [flexbox][11] and floated column generation.
* [CSS position][9] shorthand mixins.
* Expressive [CSS @media query][10] shorthand syntax.
* Media breakpoint and color variable management and retrieval.
* [Golden ratio][12] typography generation-step font sizes and line heights in tune to the prefect ratio of 1.61.
* Unitless decimal => [rem][13] generation (because).
* 20+ utility mixins to prefix values and properties, to generate gradients, modals, [counter increments][15] and [paragraph columns][14]

## Installation

    npm install charon-sass

## Usage

    @import '../path/to/node_modules/charon/charon/';

    .columns {
        @include columns(flex, div, 3, 5%);
    }

    =>

    .flex-columns-even {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    .flex-columns-even > div {
        flex: 0 1 30%;
        min-height: 1px;
    }

## Documentation
Full documentation is a (substantial) work in progress. The code comment style is compatible with [Sassdoc][6]. Execute `npm run doc` to generate HTML documentation for the project.

## TODO

* Full `@mixin` and `@function` unit test coverage with [Mocha][7] and [True][8].
* Complete this README.md file.
* Identify and remove defunct code.

<sup name="footnote-1">1: [Charon][2] is named for [Charon][3], who was named for [Charon][4], which was named for [Sharon][5], so it should be pronounced '_Shar_-on.' Easy, right?</sup>

[1]: http://sass-lang.com/ "Sass"
[2]: https://github.com/bhalash/charon "Charon (library)"
[3]: https://www.bhalash.com/archives/13544792237 "Charon (kitten)"
[4]: https://en.wikipedia.org/wiki/Charon_(moon) "Charon (moon)"
[5]: https://en.wikipedia.org/wiki/James_W._Christy "James Christy"
[6]: http://sassdoc.com/ "Sassdoc"
[7]: https://mochajs.org/ "Mocha"
[8]: http://oddbird.net/true/ "True"
[9]: https://developer.mozilla.org/en-US/docs/Web/CSS/position "CSS Position"
[10]: https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries "CSS Media Queries"
[11]: https://css-tricks.com/snippets/css/a-guide-to-flexbox/ "Flexbox"
[12]: https://pearsonified.com/typography/?utm_source=dlvr.it&utm_medium=feed "Golden Ratio"
[13]: https://www.sitepoint.com/understanding-and-using-rem-units-in-css/ "rem units"
[14]: https://css-tricks.com/almanac/properties/c/columns/ "CSS column property"
[15]: https://developer.mozilla.org/en/docs/Web/CSS/counter-increment "CSS counter increment"
