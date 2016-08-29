# Charon
Charon is a programmatic [Scss][1] library designed to give control of CSS back to individual developers. Too many Sass libraries lock you in to a their developer's preferred design paradigm-they give you pregenerated CSS or only a limited set of mixins.

Charon intends to be the counterpoint library that grants flexible, descriptive tools to developers interested in a programmatic approach to their CSS. Take the `columns` mixin:

    .columns {
        @include columns(flex, div, 3, 5%);
    }

compiles to:

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

<sup>footnote</sup>

[1]: http://sass-lang.com/ "Sass"
