[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 04- HTML Links, JS Functions, and Intro to CSS Layout

*****

## Images

Images should be relavant, convery information, convey the right mood, be instantly recognisable and fit the color palette.  

Generally images are stored in an images folder and even sub-folders organized by more specific topics.  

>add an image with `<img src="image.jpg" title="An image title" alt="An image" />`

Images can also be sized with height and with attributes.  

When creating images there are 3 things to remember :

- Save images in the right format  
  - JPEG- use for images with many different colors
  - GIF or PNG- use for images with few colors or lage areas of the same color
- Save images at the right size
- Measure images in pixels

When cropping images it is important to not lose valuable information. For example a picture of a giraffe is best in portrait orientation and should not be cropped as a landscape image.  

Vector images differ from bitmap images and are resolution independent. One way to display vector images is to save a copy in bitmap format. But a new format called scalable vector graphics (SVG) is used to display vector images directly on the web.  

Animated gifs can be used but should be limited due to file size and its effect on load speed and its perception as being amateurish.  

Transparent images can be in one of two formats:

- Transparent GIF- you can save a GIF with the transparency option selected.
- PNG- If the image has a diagonal or rounded edges or if you want a semi-opaque transparency or drop-shadow then you will need to use the PNG format.

Images often come with captions and HTML 5 has introduced the `<figure>` and `<figcaoption>` elements to support them. You can have more than one image inside a figure as long as they all share the same caption.  

## CSS Color

Text Color can be assigned in CSS with the color property `color:red`. Color also accepts RGB, Hex and HSLA values.  

Background color is set with the property `background-color:`. Default is transparent or the browser default.  

When picking foreground color and background color it is important that there be enough contrast for readability.  

CSS3 introduces the `opacity:` property whose value ranges from 0.0 to 1.0.  

## Text

Text properties that control text appearance can be split into two groups.

- Those that directly affect the font and ites appearance (typeface,bold,italic)
- Those that have the same effect on text no matter the font (color, spacing between letters and words)

The `font-family:` property allows you to specify the typeface that should be used.  
The `font-size:` property allows you to select the size of the font. Px/%/em.  
Most browsers default the size of text to 16px. So using % or em will be based off of the base text size.  

`@font-face` CSS rule allows you to use an external font. This rule has 3 properties:

- font-family- specifies the name of the font. This name can be used as a value of the font-family in the rest of the style sheet.
- src- This specifies the path to the font. May need more than one if using different formats.
- format- Specifies the format the font is supplied in. The various font formats should appear in your code in this order: 1)eot 2)woff 3)ttf/otf 4)svg  

Also checkout [fontsquirrel.com](https://www.fontsquirrel.com/fontface/generator) for converting fonts to the different formats and providing the @font-face rule.  

`text-transform:` property in a CSS rule allows value of uppercase, lowercase, and capitalize.  

`text-indent:` property allows the first line of text within element to be indented.  

`:first-letter and :first-line` pseduo-element attach after the selector and these rules only effect first line or letter.  

`:link and :visited` pseudo element that set styles to links that have not been clicked and links that have been clicked on.  

`:hover and :active` pseudo element that applies when a user hovers element and when an element is active such as when clicked.  

`:focus` pseudo element that applies to element that can be interacted with. for example when a form input is ready to accept typing or when tabbing through the page.  

> When pseudo classes are used the should appear in this order:  
> :link, :visited, :hover, :focus, :active  


## Things I want to know more about

- importing google fonts. using backup/default font families to override the browser.
- SVG usage and how to use gifs

*****

[Return to Course 201 Notes](https://KrisDunning.github.io/201/)