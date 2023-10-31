Hi Shada!

Nice work! This is really good for a first website. As you can see below you've covered most things, and most of the thing that need attention are fairly minor.

The big one, however, is the menu not being responsive. Responsiveness is the #1 thing for FE developers to focus on so I'm afraid you'll need to fix that to get a G grade. The quickest fix is to make it display as a column on mobiles, but you are free to do what you want.

So if you fix the menu on mobiles you'll get a G, to get a VG please read the comments below and try to fix them. Most are pretty quick fixes. Breaking the CSS into different files will take a bt longer - make one global.css file for all the common elements - header, menu etc - then have a index.css for the articles and see if any other page needs it's own CSS file. It's ok to have very short files. And don't forget that an HTML page can link t as many CSS files as it needs!

Please let me know when I should have another look.

*************************************

CRITERIA FOR GRADING

*************************************

GODKÄNT:
-------------------------------------

3 separate pages: ✔

A header with a page title on every page: ✔ ❌
    Kontakt & kontaktuppgifter do not have an <h1> tag. Every page should have its own unique <h1> for SEO reasons

A navigational menu every page with links to the other pages: ✔

Contact form: ✔
    Email:  ✔
    Message:  ✔
    Required:  ✔
    Mail to:  ❌
       Nice touch, but I need the action on the form to be a 'mailto: ' - I need my email client to launch when I submit the form. Check this link for an example: https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_mail

RWD:
    Desktop: ✔
    Mobile: ❌
        The menu breaks the page on mobile devices. Everything else looks good - but you need to find another solution to handle the mobile menu
External CSS: ✔

-------------------------------------

VÄLGODKÄNT:
-------------------------------------

Current page indication in the menu: ❌
   Add an "active" class or somesuch to the menu item of the current page.

Responsive Image: ✔
   Excellent

RWD:
  Media Query: ✔
     You should use a media query to make the menu responsive
  Flex/Grid: ✔ ❌
     Nice, but a few things:

     mall.css line 127:
        .column { ... } this need display: flex for the flex-column to work.

Separate CSS: ❌
   Break your css into separate pages. Mall.css is loaded on every page, which means, for example, the Kontakt page is receiving CSS for .article classes, even though the page doesn't have any articles!
  Semantic: ✔
     Very nice!

Semantic Element naming:  ✔

Code Style:
  HTML: ✔ ❌
      Generally very well done, but some odd spacing and indentation
      The header code in index.html, for example. All the elements are great but the indenting is a bit all over the place. 
      .article.tre  does not have a closing tag, which is really bad!
  CSS: ✔
      Really nice.
      Line 163 - 173 - these 3 spans all will target the same elements, so you should only have one of them!