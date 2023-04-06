# Accessibility and Inclusive Design

Objective: Students will learn the principles of accessibility and inclusive design, and how to implement them in web development. They will also learn how to use tools like screen readers and browser plugins to test the accessibility of their websites.

### What is accessibility?

**Definition and importance of accessibility in web development**

Accessibility in web development refers to designing and developing websites that can be used by people with disabilities or impairments. This ensures that all users, regardless of their abilities, can access web content and services. Accessibility is crucial because it promotes inclusivity, improves user experience, enhances search engine optimization, expands the reach of a website, and mitigates legal risks. By ensuring accessibility, web developers can create a more inclusive digital world where everyone has equal access to information and services.

**Laws and regulations related to accessibility (e.g. Americans with Disabilities Act)**

It is important for web developers to be aware of laws and regulations related to accessibility, such as the Americans with Disabilities Act (ADA), Section 508 of the Rehabilitation Act, and the Web Content Accessibility Guidelines (WCAG). These regulations ensure that websites are accessible to individuals with disabilities, such as those who are blind or have low vision, deaf or hard of hearing, or have physical or cognitive disabilities. Compliance with these laws and regulations not only ensures equal access for individuals with disabilities but also mitigates legal risks for businesses and organizations. Therefore, web developers should incorporate accessibility into their development process to ensure compliance with these regulations and promote inclusivity for all users.


**Common barriers to accessibility (e.g. visual, auditory, motor impairments)** 

Accessibility barriers are obstacles that prevent individuals with disabilities from accessing and using digital content and services. Common barriers to accessibility include visual impairments, such as blindness or low vision, auditory impairments, such as deafness or hard of hearing, and motor impairments, such as difficulty using a mouse or keyboard. Other barriers may include cognitive or neurological impairments, such as dyslexia or autism, or environmental factors, such as poor lighting or loud background noise. These barriers can prevent individuals with disabilities from fully participating in the digital world, including accessing educational resources, conducting online transactions, and engaging in social media. To ensure accessibility for all users, web developers should consider these barriers when designing and developing digital content and services and provide alternative formats or assistive technologies to accommodate different types of disabilities.

### Inclusive design principles

- Designing for diversity and inclusivity

Suppose a web developer is creating a new e-commerce site. To ensure diversity and inclusivity, the developer could design the site's interface to be easily navigable using assistive technologies, such as screen readers, for users with visual impairments. They could also provide alternative formats for visual content, such as image descriptions, to make the content accessible to users who are blind or have low vision. Additionally, the developer could consider the language and cultural background of the site's target audience, using clear and concise language and avoiding cultural stereotypes that could exclude certain groups of people. Finally, the developer could conduct user testing with people from a diverse range of backgrounds and abilities to ensure that the site is usable and accessible to as many people as possible.

Why?

Designing for diversity and inclusivity is important because it ensures that digital content and services are accessible and usable by the widest possible audience. By considering the needs of individuals with different abilities, cultural backgrounds, and experiences, web developers can create content and services that are more inclusive, welcoming, and engaging to a broader range of people. This can lead to increased engagement, better user experiences, and ultimately, greater success for businesses and organizations. Moreover, designing for diversity and inclusivity promotes ethical and moral principles of equality and social justice, contributing to a more inclusive and equitable society.

**Prioritizing user needs and preferences**

Prioritizing user needs and preferences in web development involves understanding and designing for the goals and behaviors of the website's target audience. This approach is user-centered and puts the needs and preferences of users at the forefront of the design process. User research and feedback are essential for identifying user needs and preferences and determining which features and functionalities are most important to them. This information can inform the design and development of the website, ensuring that it meets the needs and preferences of its users.

Prioritizing user needs and preferences is important because it leads to a better user experience and higher user engagement. When users can easily find the information or services they need and the website is designed in a way that resonates with them, they are more likely to spend time on the site, return to it in the future, and share it with others. Moreover, user-centered design can lead to a competitive advantage, as users are more likely to choose a website that meets their needs over one that does not. Therefore, prioritizing user needs and preferences is a key consideration for web developers who want to create effective and successful websites.


**Providing multiple ways to access information and perform actions**

Providing multiple ways to access information and perform actions is an important consideration in web development to ensure that all users, regardless of their abilities or technological limitations, can access the content and functionalities of a website.

Multiple ways of access could include providing alternative text descriptions for images, videos or other visual content, so that users with visual impairments can understand what is being displayed. Another example could be offering keyboard shortcuts and alternative input methods, such as voice commands or touch gestures, to accommodate users with mobility impairments who may not be able to use a mouse or standard keyboard.

Providing multiple ways of access is important because it ensures that all users can interact with a website, regardless of their abilities or technological limitations. This promotes inclusivity and reduces the risk of exclusion, which can occur when a website is designed with only one type of user in mind. By providing multiple ways of access, web developers can ensure that users with disabilities, as well as those who may have limited access to technology or slow internet connections, can still engage with a website and its content in a meaningful way. This can lead to increased engagement and satisfaction for all users, regardless of their backgrounds and abilities.

### Techniques for accessible web development

- Semantic HTML - You've used this before! 
- Alt text for images - You've also seen this!
- ARIA attributes
- Proper use of color and contrast
- Keyboard navigation
- Captions and transcripts for video and audio content

**ARIA**

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

### Tools for testing accessibility

- Screen readers (e.g. NVDA, VoiceOver)
- Browser plugins (e.g. WebAIM's WAVE tool)
- Keyboard-only navigation

https://wave.webaim.org


Accessability for React 

https://blog.bitsrc.io/5-web-accessibility-tools-for-react-applications-e1baad7c6087

Install: axe-devtools-web accessibility testing

https://chrome.google.com/webstore/detail/axe-devtools-web-accessib/lhdoppojpmngadmnindnejefpokejbdd/related?hl=en-US&utm_term=chrome%20accessibility%20checker&utm_campaign=Search%20-%20axe%20DevTools%20-%20Checker&utm_source=adwords&utm_medium=ppc&hsa_src=g&hsa_ad=552272061977&hsa_tgt=kwd-1464153033563&hsa_mt=e&hsa_ver=3&hsa_acc=7854167720&hsa_kw=chrome%20accessibility%20checker&hsa_grp=135123751344&hsa_cam=14920961979&hsa_net=adwords&gclid=EAIaIQobChMIgpebrpHr_QIVUACtBh0mXAqxEAAYASAAEgKOn_D_BwE

Open your page in Chrome, next open the Inspector and find axe devtools. Run the accessiblity test. 

Use the color constrast checker:

https://webaim.org/resources/contrastchecker/

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




HOMEWORK

find a web site, a site that exists out in the world, something you use every day, try and use that website only using a screen reader. 