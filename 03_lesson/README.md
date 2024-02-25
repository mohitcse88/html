# HTML 
## 03 TEXT BASICS

### Web Pages they are :- 
- **Essays** or Even a **Newpaper** where they have headings and usually paragraphs of text
- or at least a sentence or two of text describing something afterwards so we see our paragraph 
- Much of text content on a web page will be made up of **headings** and **paragraph**
- Now headings have hierarchy and that and that means we will start out with **only one h1 on the page and each page should have one h1** but after that we can have sub topics

### heading h1 , h2 - Flow the Hierarchy 
- Imagine this being the title of the essay or the big headline in the newspaper and then we have subtopics like h2 h3 ...
- We could have more than one h2 on the page but I wanted to show how you could have sub topics or h3 under the sub topics or h2 so we have title for our essay 
- h1 - Title for essay 
- h2 - area of discussion 
- Screen reader or other assistive technology looks at our code then it can navigate the code through the headers of what important here the header hierarchy and that's why It's so important to organize your page the headers actually give semantic meaning saying this is the main topic this is the sub-topic under the main topic and this is the sub-topic under the higher sub-topic in the heirarchy so headers do have semantic importance and means giving menaing to our content. 

### Paragraph 
- paragraphs can just have whatever details we want to add about those subtopics 

### Non - semantic meaning 
- hr - horizontal row 
    - an element that doesn't really provide any semantic meaning but visually it helps us on the page and that is a horizontal rule element

### White Spaces
- space is web pages or html do not honor all those spaces you might add with a space bar it's called white space collapsing and so we can space many lines but it won't really be represented on the page that is not how we add extra space in html 

### br - line break
- p - we don't have to have the opening and closing tags on the same line for an element for paragraph
- 
we can nest other elements inside of an element
***
## Block Level Elements 
- Here Every Pragraph and Every Heading they start on a New line that is a block Level Elements it creates space around it 
    - we can formated with css 
- But It doesn't allow to put another paragraph inside of a header or a pragraph without creating a new line that spaces so there will be return essentially in your content when we are using a Block level element but when we use inline element that doesn't happen 
### h1  to h6
### p
### address 
    - All text will italicized by default
    - address element and we can put a location inside of this address element and it tells the browser that this is an address or a specific location
    - assistive technology so an address element does provide some semantic meaning as well to the content within it
***
## Inline Element 
### em 
- It has some semantic meaning 
- When screen reader or other assitive technology or just our browser overall knows we are empahsizing this really need a getaway so let's save and notice really need a getaway is italicized
- text again the formatting will come later with CSS but that is just the natural behavior of using the emphasis element
### strong 
- it provides that meaning now what if we really want to emphasize that text it has a strong meaning to us 
- It makes text to little bit bigger and bolder here as far as the natural formatting of the strong element
### abbr
- acronym or abbreviation for the Mozilla developer network (MDN)
- when we hover our mouse on MDN we got tooltip that says Mozilla developer network
- **tooltip** 
    - tooltip will not really be available to screen reader and assistive technology so we don't want anything super important for the understanding of the meaning of the page to be in there so if we are using abbreviation it's a nice thing to have but it is really not accessible to all assistive technology so it's you can't have anything in there that the page really depends on because some of the people accessing the page may not be able to read or see the information that you provide here inside the title attribute of the abbreviation element
***
## HTML Entities 
- HTML entities so they are things that are not really the normal text we would type out what for example if we wanted to show a less than or a greater than symbol on our page right now HTML interprets those as we're starting or ending a tag
- So we can't just easily put one of those on the page likewise there are some other symbols
- white space collapsing if we need a little bit of extra space there's an HTML entity for that 
### HTML Entities Writing 
- ampersand (@) is usually what starts out an HTML entity 
### @nbsp; 
- It add whites spaces in the web pages

### lt 
```
&lt;
``` 
- lt stands for less than (<)

## HTML COMMENT
- we won't see it on the page but it is important to us and this is an HTML comment
- I will show you how the public can see this if we right click and choose inspect that works or you can also press ctrl u either way will show your source code now notice we've got a comment
-  **live server** also injected a comment here and it injected some javascript so when we look at the overall source code of what is live
- so just to let you know if you leave a note for yourself it can be viewed by others