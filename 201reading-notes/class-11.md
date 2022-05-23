[Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 11- Audio, Video, Images

*****

## Images

Setting an image size is as easy as specifying the CSS value of height and width. Common image sizes are often :

- small portrait : 220x360
- small landscape : 330x210
- feature photo : 620x400

A good way to implement shared common size attributes is to give the image and a class in the HTML document like small, medium or large. Then set the height and width of those classes in your CSS.  

Two common ways to align images using CSS are:

- 1) Set the `float` property to the class that represents the size of the image as stated above
- 2) New classes are created with names such as align-left or align-right to use for aligning the images.

It is also common  to add a margin to the image to ensure that the text does not touch their edges. 

By default images are inline elements. Im orger to center an image it should be turned into a block level element, then either use `text-align: center` on the containing element or on the image itself set the `margin` values of left and right to auto. 

## Background Images

Background images are often the last thing on the page to laod. If the file is too large then it will take longer to load and may make the page appear slow to load. Background image porperties that can be set:

- repeat- the background image is repeated both horizontally and vertically (default)
- repeat-x- image is repeated horizontally only
- repeat-y- image is repeated vertically only
- no-repeat- image is only shown once. 

The background-attachment property specifies whether a background image should stay in one position or mave at the user scrolls up and down the page. It can have one of two values:

- fixed- image stays in same position on the page
- scroll- image moves up and down as the user scrolls up and down the page  

### Background-position

When an image is not being repeated you can use the background-position property to specuf where un the browser window the image should be placed. The property usually has a pair of values. The first represents the horizontal and the second the vertical. Options are:

- left top, left center, left bottom
- right top, right center, reight bottom

You can also set a pair of pixels or percentages. These represent the distance from the top left corner of the browser window (or containing box). 50% 50% is centered for example. 

### Image rollover and sprites

Using CSS it is possible to create a link or button that changes to a second style when a user moves their mouse over it (rollover) and a 3rd style when they click it. 

This is achieved by setting multiple images with different stylings that can be moved or switched between to achieve the effect. Single images used for several different parts of an interface is known as a `sprite`. 

### Gradients and Background Image Contrast

CSS allows us to specify a gradient for the background of a box. The gradiant option is not covered in detail in this textbook but MDN has a reference page available for more information. 

Most photographs have high contrast and are not ideal for use as a background image. A low contrast background image makes text above it easier to read. To overlay a high contrast image you can place a semi-transparent backgroun color (a screen) behind the text to improve legibility.  

## Search Engine Optimazation (SEO)

### The basics

SEO is the practice of trying to help your site appear nearer the top of search engine resultys when people look for the topice that your website covers. At the heart of SEO is working out which words people use to search for your site. Then using those terms in the right places on your site to increase chances search engines show a link to your site. Search engines dont just search your site they also see how many sites link to you and how relavent those links are. For this reason SEO is often split into two areas, on-page techniques and off-page techniques.  

### On-Page techniques

These are the methodds you can use on your web pages ti improve their search rating. The main component is the search words to find your site. Imclude those words in the text and HTML of the page. Seach engines rely heavily on the text on your web pages. There are 7 key places to place these keywords:

- Pagge title
- URL/Web address
- Headings
- Text
- Link Text
- Image Alt Texts
- Page descriptions

Dont try to be tricky. Search engines know the common tricks. Be genuine. 

### Off-Page techniques

Getting other sites to link to you is just as important as on0page techniques. Search engines are particularly interested in sites whose content is related to yours. Search engines also look at the words between the opening and closing `<a>` tags. If there are keywords they may be considered more relavent. Text that appears in links of the page should also apprear on the site it links to.  

### Google Analytics

One of the best tools to analyze how people found your site, what they are looking at and at what point do they leave is a free service called Good Analytics.  

### Domain Names and Hosting

To put your website on the web you will need a domain name and web hosting.  

Domain names- Your domain name is your web address. Usually there is an annual fee to retain your domain name. Sites that offer domain name registration often offer web hosting as well.  

Web Hosting- For other people to see your site you will need to upload it to a web server. They are special computers that are constantly connected to the internet. They are specially set to serve pages when requested. Most web sites are hoted by web hosting companies. Some things that may determine which hosting company is best for your are:

- Disk space- total size of all the files that make up your site. HTML,CSS,JS,Images.
- Bandwidth- Amount of data the company will send to your site's visitors.
- Backups- Whether the company performs backups on your site and how often. Some only create backups for mechanical server failure and some allow you to access in the event of you accidentally breaking your site when updating it. 
- Email Accounts- Most hosting companies will provide email servers along with their hosting package. Check the number of mailboxes and size of storage. 
- Server-side languages and databases- If you are using a content management system (CMS) it will likely use a sever side programming language and a database. Be sure to check that your hosting company supports the technologies your software needs to run.

### FTP and Third Party Tools

To transfer your code to the server you use a file transfer protocol (FTP). There are many FTP programs that offer simple interfaces that will both your local files and the files hosted on your server. Some hosting companies may offer a web based tool but usually FTP is quicker. You will receive FTP details from the web hosting company which usually be an FTP address, a username and password.  

## Things I want to know more about

animations and how the canvas elements interact with .gifs and standards for audio effects inclusion. No audio or video in the reading? iFrames and embedding video (copyright issues?)

*****