<style>
  body {
  margin: 2em auto;
  max-width: 80%;
  font-family: sans-serif;
  font-size: 20px;
  }

  .swatch {
    display: inline-flex;
    align-items: center;
  }

  .swatch::before {
    display: inline-block;
    width: 2em;
    height: 2em;
    background-color: #000000;
    margin-right: 1em;
    content: " ";
  }
  </style>
<body>

## Colour swatches

Each swatch should include:

1. visual representation of the colour, typically a colour filled box.
2. a hex value for the colour, ie: `#000000` is black
3. the name of the colour

Example:

  <div class="swatch">
  #000000, Black
  </div>

You should include swatches for:

1. Primary colour, typically from the brand
2. Secondary colour, typically from the brand
3. Accent colour
4. Neutral colours, used for text, backgrounds - most of the UI is neutral colours
5. Semantic colours, these are colours that have meaning to users. For example, success, error, warning, info and danger alerts.
6. Extended colours, these are typically tints and tones of your primary and secondary colours

## Typography swatch

In a typography swatch, you identify the fonts you will use and how you will use them.

For different elements of your site, identify the font, font-weight and size that will be user.

You want to define this for:

- All heading levels
- body (paragraph text, asides, quotes)
- navigation
- form elements (labels and buttons)

You should also include variants such as small, medium and large variants of elements.

For example:

**Body | Paragraph**

_Default_

- Font: Comic Sans
- Size: 18px
- Weight: regular

_small_

- Font: Comic Sans
- Size: 14px
- Weight: thin

_Large_

- Font: Comic Sans
- Size: 24px
- Weight: medium

</body>
