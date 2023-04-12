# Accessibility Part 2

Modifying an existing site to improve accessibility. 

## ARIA

ARIA (Accessible Rich Internet Applications) attributes are HTML attributes that can be used to improve the accessibility of web content for individuals with disabilities. These attributes can be added to HTML tags to provide additional information about the function, purpose, or state of an element, such as a button, form, or widget.

ARIA attributes include roles, which define the type or category of an element, such as "button", "listbox", or "menu", and states, which describe the current condition or value of an element, such as "selected", "disabled", or "expanded". ARIA attributes also include properties, which provide additional information about an element, such as "aria-label" to provide a label for an element or "aria-describedby" to provide a description of an element.

Using ARIA attributes can improve the accessibility of web content by making it easier for individuals with disabilities to interact with a website. For example, ARIA attributes can help screen readers interpret the purpose and function of different elements on a webpage, allowing users with visual impairments to navigate and interact with the content more easily. By providing this additional information, web developers can ensure that their websites are accessible to a wider range of users, including those with disabilities.

**ARIA examples**

ARIA role for navigation menus: If a website has a navigation menu, it's important to make sure that it is accessible to all users, including those who use screen readers. One way to do this is to use the ARIA role attribute to identify the menu as a navigation landmark. For example, the following code could be used to mark up a navigation menu with the ARIA role of "navigation":

```HTML
<nav role="navigation">
  <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">About</a></li>
    <li><a href="#">Contact</a></li>
  </ul>
</nav>
```

By adding the role attribute with a value of "navigation", screen readers will be able to identify the navigation menu as a distinct landmark on the page, making it easier for users to navigate to the content they are looking for.

ARIA attribute for form inputs: Forms are an important part of many websites, but they can be challenging for users with disabilities to complete. ARIA attributes can help make forms more accessible by providing additional information about form inputs. For example, the following code could be used to add a label and description to a text input field:

```HTML
<label for="name">Name:</label>
<input type="text" id="name" aria-describedby="name-description">

<span id="name-description">Enter your full name.</span>
```

In this example, the "for" attribute on the label element is used to associate the label with the input field, while the "aria-describedby" attribute on the input element is used to associate it with a description of the input field. Screen readers can then read out the label and description together, making it easier for users to understand the purpose of the input field.

Take a look at the ARIA attributes page over at Mozilla: https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA

React docs also have an ARIA page, you should read this: https://legacy.reactjs.org/docs/accessibility.html

https://www.lullabot.com/articles/what-heck-aria-beginners-guide-aria-accessibility

### Color and contrast 

Contrast is the difference in value between two colors. The value of a color is how dark or light a color would appear if you converted it to gray scale. Red for example is is about 50% gray. Blue is often darker and yellow is often lighter. 

It's the value difference that that makes things stand out and the lack of contrast makes things harder to read.

Contrast has been rated for accessibility. Use this site to check your colors. 

https://webaim.org/resources/contrastchecker/

NOTE! For text font size and weight matter. Smaller fonts, and lighter weight fonts are harder to read and require more contrast! Becuase two colors work at one point size doesn't mean they are legible to everyone at every point size. 

Accessability for React 

https://blog.bitsrc.io/5-web-accessibility-tools-for-react-applications-e1baad7c6087

Install: axe-devtools-web accessibility testing

https://chrome.google.com/webstore/detail/axe-devtools-web-accessib/lhdoppojpmngadmnindnejefpokejbdd/related?hl=en-US&utm_term=chrome%20accessibility%20checker&utm_campaign=Search%20-%20axe%20DevTools%20-%20Checker&utm_source=adwords&utm_medium=ppc&hsa_src=g&hsa_ad=552272061977&hsa_tgt=kwd-1464153033563&hsa_mt=e&hsa_ver=3&hsa_acc=7854167720&hsa_kw=chrome%20accessibility%20checker&hsa_grp=135123751344&hsa_cam=14920961979&hsa_net=adwords&gclid=EAIaIQobChMIgpebrpHr_QIVUACtBh0mXAqxEAAYASAAEgKOn_D_BwE

Open your page in Chrome, next open the Inspector and find axe devtools. Run the accessiblity test. 

Install Lighthouse chrom extension: 

https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk

OPen the inspector and find lighthouse and run the test. You'll need to run the test on all of your "pages" for example the home page, the about page, and one of the detail pages. 

## Screen readers 

To really get a feel for how people with disabilities use a computer try the screen reader. 

- Safari: https://www.apple.com/voiceover/info/guide/_1121.html
- Chrome: https://support.google.com/accessibility/answer/7031755?hl=en

## Challenge

**Challenge** Browse your website using the a screen reader. See if you understand your website with the screen reader. 

When the screen read is active you can click on things. The screen read should read each item. 

If you are unable to use the mouse you'll use the keyboard to navigate. This can be especially frustrating. Put your developer hat on for a few minutes, is if you ever take it off. You can move through each element on the page using the arrow keys. You can also move through navigational and control elements like buttons and text inputs using the tab, and option + tab, and the shift key and you can mobe backwards. 

To enabled tabbing through the links on a page, in Chrome use the tab key, in Safari use option + tab. 

Notice the order things on the screen as you tab over them. Does this makes sense? You can control the tab order using the `tabindex` attribute. Read about it here: https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/tabindex

Spend some time playing with this. It gets frustrating really fast. Think about how it would be to use this every day. The challenge is to think of how you can make reduce the frustration of this process through the design of your site! 

Think of at least three ways you can improve the accessibility of your site. 

**Challenge** use lighthouse to score your pages. You can do as much work on your site as you like. I will score this assignment on the lowest scoring page. My solution project from the tutorial scored 81%. 





Accessability for React.

https://blog.bitsrc.io/5-web-accessibility-tools-for-react-applications-e1baad7c6087

Install: [axe-devtools-web accessibility testing](https://chrome.google.com/webstore/detail/axe-devtools-web-accessib/lhdoppojpmngadmnindnejefpokejbdd/related?hl=en-US&utm_term=chrome%20accessibility%20checker&utm_campaign=Search%20-%20axe%20DevTools%20-%20Checker&utm_source=adwords&utm_medium=ppc&hsa_src=g&hsa_ad=552272061977&hsa_tgt=kwd-1464153033563&hsa_mt=e&hsa_ver=3&hsa_acc=7854167720&hsa_kw=chrome%20accessibility%20checker&hsa_grp=135123751344&hsa_cam=14920961979&hsa_net=adwords&gclid=EAIaIQobChMIgpebrpHr_QIVUACtBh0mXAqxEAAYASAAEgKOn_D_BwE)



HOMEWORK

find a web site, a site that exists out in the world, something you use every day, try and use that website only using a screen reader. 


























https://dev.to/devsatasurion/is-tailwind-css-accessible-52dc

Tailwind Screen Readers 
https://tailwindcss.com/docs/screen-readers


TailwindCSS color and WCAG color scores

https://colour-a11y.vercel.app


A11y - Needs a definition
accessibility -> a(eleven letters)y a ccessibilit y
a11y -> Ally
https://en.wiktionary.org/wiki/a11y

ARIA attributes - Is this covered? 
Accessible Rich Internet Applications 


--------------------

React Accessability:

https://legacy.reactjs.org/docs/accessibility.html


WUHCAG Checklist - 
https://www.wuhcag.com/wcag-checklist/
How many of these things can you find in your project? 

