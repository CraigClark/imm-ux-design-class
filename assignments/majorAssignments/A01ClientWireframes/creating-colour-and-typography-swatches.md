<style>
  body {
  margin: 2em auto;
  max-width: 80%;
  font-family: sans-serif;
  font-size: 20px;
  }

  .swatch {
    display: flex;
    align-items: center;
  }

  .swatch::before {
    display: inline-block;
    width: 2em;
    height: 2em;
    margin-right: 1em;
    content: " ";
  }

  .black::before {
    background-color: #1e1e1e;
  }

  .white::before {
    background-color: #ffffff;
    border: 1px solid #1e1e1e;
  }

  .primary::before {
    background-color: #38761d;
  }

  .primary-tint-1::before {
    background-color: #ebf1e8;
  }

  .primary-tint-2::before {
    background-color: #c3d5bb;
  }

  .primary-tint-3::before {
    background-color: #9bba8e;
  }

  .primary-shade-1::before {
    background-color: #326a1a;
  }

  .primary-shade-2::before {
    background-color: #275214;
  }

  .primary-shade-3::before {
    background-color: #1c3b0e;
  }

  .comic-sans {
    font-family: "Comic Sans MS", "Comic Sans", cursive;
  }

  </style>
<body>

## Colour swatches

Each swatch should include:

1. visual representation of the colour, typically a colour filled box.
2. a hex value for the colour, ie: `#000000` is black
3. the name of the colour

Example:

  <div class="swatch black">
  #1e1e1e, Black
  </div>

You should include swatches for:

1. Primary colour, typically from the brand
2. Secondary colour, typically from the brand
3. Accent colour
4. Neutral colours, used for text, backgrounds - most of the UI is neutral colours
5. Semantic colours, these are colours that have meaning to users. For example, success, error, warning, info and danger alerts.
6. Extended colours, these are typically tints and tones of your primary and secondary colours

Make sure you have a naming convention for each colour to reference in the wireframe description. For example:

**Global colours**

  <p class="swatch black">
  #1e1e1e, Black
  </p>

  <p class="swatch white">
  #ffffff, White
  </p>

**Primary and variants**

<p class="swatch primary">
  #38761d, Primary
</p>

<p class="swatch primary-tint-1">
  #ebf1e8, Primary tint 1
</p>

<p class="swatch primary-tint-2">
  #c3d5bb, Primary tint 2
</p>

<p class="swatch primary-tint-3">
  #9bba8e, Primary tint 3
</p>

<p class="swatch primary-shade-1">
  #326a1a, Primary shade 1
</p>

<p class="swatch primary-shade-2">
  #275214, Primary shade 2
</p>

<p class="swatch primary-shade-3">
  #1c3b0e, Primary shade 3
</p>

## Typography swatch

In a typography swatch, you identify the fonts you will use and how you will use them.

For all elements of your site, identify the font and font-weight the element uses.
For example:

- All heading levels
- body (paragraph text, asides, quotes)
- navigation
- form elements (labels and buttons)
- captions
- links

You should also include variants such as small, medium and large variants of elements.

For example:

**Primary font**

_Primary default_

- font: <span class="comic-sans">Comic Sans</span>
- weight: regular

_Primary sm_

- font: <span class="comic-sans">Comic Sans</span>
- weight: thin

_Primary lg_

- font: <span class="comic-sans">Comic Sans</span>
- weight: medium

_Primary xl_

- font: <span class="comic-sans"><b>Comic Sans<b></span>
- weight: bold

> ## Describing elements in a wireframe
>
> It is important that team members understand the appearance of every element on a page.
>
> **Example**
> I have a header with the following elements:
>
> 1. logo
> 2. title
> 3. search bar
> 4. user account (icon and text)
> 5. shopping cart icon
> 6. hamburger nav
>
> To describe these, I need to know what fonts, colours, and any other details used to make the element.
> For this example, I have my colours and fonts described above, however, I need to describe borders and radius as well. So I add:
>
> ### Border styles
>
> - **Border sm**: 1px solid
> - **Border md**: 2px solid
> - **Border lg**: 4px solid
>
> ### Radius styles
>
> - **Raduis 1**: 5px
> - **Raduis 2**: 10px
> - **Raduis cr**: 50% (circle)
>
> I would describe my header element like this:
>
> ### Header
>
> background colour: Primary tint 1  
> border bottom: Border md  
> border bottom colour: Primary shade 3
>
> **Header > title**  
> colour: Primary  
> typography mobile: Primary xl, 20px (note that I added the size here)  
> typography desktop: Primary xl, 30px
>
> **Header > search > input**  
> background colour: White  
> color: Black  
> typography mobile: primary default: 18px  
> typography desktop: primary default: 20px  
> border sm  
> radius mobile: radius 1  
> radius desktop: radius 2
>
> **Header > search > button**  
> background colour: Primary shade 2  
> icon colour: Primary tint 1
>
> **Header > user account**  
> icon colour: Primary shade 2  
> typography mobile: primary small: 16px  
> typography desktop: primary small: 18px
>
> **Header > shopping cart**  
> icon colour: Primary shade 2
>
> **Header > nav**
> icon colour: Primary shade 2
>
> _Notice that I did not describe the logo. This is because it is an image and will appear on the wireframes as a circle with an X in it. There is no need to describe it here. The user can understand by looking at the wireframe_

</body>
