# HTML
## Semantic Tags
Documents need organization and our html files are no different html achieves document organization with Semantics

## Heading Tags Writing HTML
Hierarchy of headers you only want one h1 per page and this should be an outline much like you would have an outline for an essay or any type of paper topic you would write so this is your title for the whole page essentially and from there you can have multiple h2 headers which is one level down in the hierarchy and they would define sub topics and then beneath that you could have h3 headers if there was a sub topic of a sub topic and so on and that continues to h6 although you really don't want any more than about **three levels of headings on a page** so h1 h2 h3 would be the ideal way to have a page laid out 

after that we need to consider some things about semantic html **writing semantic html helps us quickly see or read the different sections in a web page and navigate to those sections**
***

## nav
nav elements are semantic elements
***

## hr
hr which stands for horizontal rule in the past i believe i might have said these didn't really have a semantic meaning but they do they're currently viewed as semantic elements and it means that there is a topic change so something is changing and of course we have a couple of topics on our page and we have horizontal rules between those  in the future as we learn css we may want to remove the horizontal rules we see here that divide our navigation and our heading for the page and replace those with lines that we can create with css because we're not really separating topics here although it doesn't hurt to have these horizontal rules in place at this time
***

## semantic 
the main thing to convey about semantic html is the word semantic that means it provides meaning as the nav element says hey this is a navigation area or the h1 element says hey this is a heading we can also get that from other parts of the page we added section elements that say this is a new section so they provide additional meaning rather than just
a generic divider and we will talk about what a generic divider is later as well now in addition semantic html makes our pages accessible to screen readers and other assistive technology and that is very important as we create pages

## header 
header for our page now we have a heading which is the title of the page but we can wrap this in a header element and there can be more than one header element per page however it needs

to follow the heading hierarchy so imagine if we had a social media site now every post whether it would be a blog post or a post like facebook or instagram every post could have its own header and it might have a subtitle in that post as well but this is a header now for our full page so this would be at the top level of our page with the hierarchy here of h1 which is the heading for our page notice we've also included the navigation inside of our header and we can go ahead and remove this horizontal rule and i think it will be just fine we don't need the semantic meaning of a

change topic there and i think it's going to look okay without the line as well so let's save this now and we can see live server updates our page immediately so we can see the change and really all we see visually is that our horizontal rule is removed however we have added some extra meaning to our html here now that this is the heading or the header section for our full page 

## main 
main element now there can only be one main element per page and by definition that would make sense you can only have one main area for content per page and so we'll start here and it's going to include our sections that we've created so i used control x to cut the closing main element tag and i'll scroll down to where our second section ends before our area here at the end and i'll paste the closing main element and save and we can see visual studio code reformatted for us so now we've got the main element wrapping our two topic areas of vacation and of html so we've added a header and a main element 

## footer
footer now just like the header there can be more than one footer per page and that might be a footer for a blog post or a footer for a social media post but this is the footer for our entire page in this example once again control x to cut that closing tag and i'm going to wrap everything we have here at the end in the footer one other thing i want to add just because i didn't do it before we validated our page throughout the other lessons and it's not an error it's not a problem but i want to include this information here about the copyright i want to include that in a paragraph element so 
i'm going to make sure that's lowercase what am i getting a capital there we go and then i'm going to once again cut the closing tag and put it after the content and save it gets reformatted it really doesn't change the look i just wanted both inside that paragraph and that might help in the future when we want to format this area as well with css

##

so now our document has been outlined into three major sections we have a footer a main area and a header and then inside the header we've already discussed we have a navigation element that is also semantic html
2:08:22
our list is also semantic html we know right away that this is providing a list and this would be identified by assistive technology as well now there can be more than one nav element per page so we might have a nav area in the footer footers often have links to other areas of a website now we've only got a couple of links in our footer and one goes back to the top and the other does go to our about page however it's not a grouping of links where we would organize if we had several other things here i might consider a nav and if you do have more than one nav element per page
2:08:59
it's important that they are labeled so assistive technology knows which nav is which and here we can do that with an attribute called aria-label and then we can set it equal to something that clearly says what it is like primary navigation and

now we have labeled our nav as the primary navigation area if you did include a heading in the nav element which is not required but if you did you could link to that so you could have an h2 here and then in the h2 we might put primary navigation if i can spell it there we go and now let's give this an id
2:09:47

and here we'll give the id the same value primary navigation and then here instead of aria we would say aria labeled by is the correct attribute here now we're looking at our primary navigation value and it's saying hey it's labeled by this value that's in the h2 so you can link these together with an aria labeled by pointing back to the id of a heading 
```
<nav aria-labelledby="primary-navigation">
<h2 id="primary-navigation">Primary Navigation</h2>
```
however since we're not going to have an h2 in our nav i'll go ahead and remove that and you can just choose the aria label attribute and set that equal to primary navigation which is equally accessible to screen readers and other technologies 

## article and section 

main area previously we broke our topics html and vacation into sections which are semantic html tags however there is a more appropriate tag now that we kind of have an idea of how our page is laid out because these are areas that could be on their own maybe they would each have their own page but much like a social media post or a blog post some type of article you might think there is an article element so i have
2:11:11
highlighted this section and i'm going to type article instead and i believe we'll find that vs code changes our closing tag immediately yes and it was already changed to article so instead of a section let's call this an article because it clearly has its own topic and now let's do the same for our other section based on vacation so we can highlight it change it to article and we'll verify that the closing tag is also article and yes it is right here so now we have two articles instead of sections now there is sometimes a debate about
2:11:48
which should be used and it's really not clearly defined if article or section is the proper choice they would both pass a validator check so really the way i look at it is an article has a clear topic where a section is more generic you might use a section just to actually create a little section in your code whereas an article has a clear topic that the area is about so now inside of the article we could create other articles but now i want to go ahead and add a couple of sections inside of our html article so as our article begins we've got the heading which is h2 and

##
h1 being the heading for the overall page the h2 being the heading for the article and then the h3 article being the headings for the nested sections within the article so we're keeping our hierarchy in 

## aside
aside as the sidebar to the page but it could also just be another section of complementary text 
that is not as important as what's in the main section or article that you are putting it inside of and that's what we'll do here and then i want to use some other semantic elements just to demonstrate how they work so now i'm going to add a detail semantic element and inside a details element you want to add a summary element now the summary if this was a product we might just put warranty information in here as the summary here i'm going to put something that's more like a question and it will display how the details and summary work so i'm going to say guess the number


of hours i code per day as our summary now underneath we can put the answer to this question and now i'm going to put i start at 8 am and i write code for let's say three hours every morning and we can save that i'll scroll up so we have it up here towards the middle of our page and now let's scroll up here and let's look at what we have on the page because the rest of our semantic changes really didn't change the appearance here but this where we added this new content notice we're not seeing this paragraph at this point we just see guess the number of hours
2:15:45
i code per day but it has this little arrow next to it if we click on this then we see the answer so that's a nice little addition that this html element adds and again these are all semantic elements so the aside has some meaning that it's complementary text it's not as important as what's in the rest of the article the details and the summary work together so this could once again provide details about a product say warranty information something else the return policy whatever but you could also use it kind of as a quiz here where you have a question and an answer


let's go ahead and add just a couple of more semantic elements to this one is what we can do with a highlighter just like you might use a highlighter on a piece of paper there is an element called mark so i'm going to mark what i want to highlight here in the text and by including it in the text you know it's an inline element and not a block element so now if i save that we have highlighted number of hours now inside the answer we're looking at some time here we have 8am and we also have a duration of three hours we can add some meaning to that in the text
2:17:03
as well and we can provide a time element then we need a date time attribute and for the date time attribute value i want to put in the actual hours it accepts several values so this would be 0800 on a 24 hour clock and now let's put the closing time element after the 8am here and notice if i save this right now and show this it does not change what 8am looks like at all but once again it provides meaning in our html for technologies that are reading it especially those assistive technologies but it could also provide some meaning for the browser itself now also it says
2:17:47
as i write code for three hours we can provide a time element for the duration too so we have time once again with the date time attribute and now we'll put in a different value because there is a value for duration i'm going to put this closing tag at the end of the three hours now let's look at the value for duration we would put in pt3h and remember there is a link in all of the html resources that i link to in the description there is a link that shows all of the html elements so you can look up for example the time element on the mozilla developer network that's the mdn site
2:18:26
and you can look at all the values that could be accepted for the date time attribute okay let's save this

##
it doesn't change the look but it does change how the browser interprets and it definitely adds a benefit for assistive technology

##
our document outline with these changes


## div
```
<div></div>
<span></span>
```
two different elements that you want to avoid as you're learning html and then later on you can use them as we possibly get into them with css but there is a div in an older html code you will see divs everywhere sometimes you still do when those people that have been using divs are used to still writing them and they just continue what they've been doing in the past however there is no semantic meaning to a div think of a div much like a section without the semantic meaning it just stands for divider and really you can put them anywhere but if you do you really have to do a lot of work to get them to convey meaning you have to add additional attributes that help assistive technology interpret these elements because they have no meaning as is they are block elements

## span 
so a very similar element that is an inline element if we just wanted to wrap a word or two in a paragraph in an element is span we'll definitely use some spans as we learn css however once again they have no meaning whatsoever by themselves they don't change or add any value to your code and we would use them possibly to apply 

##
2:21:07
some css styling to some words that we would highlight around span so we really want to avoid both of these elements as you learn html really work on using semantic elements and then when you understand what semantic elements are and how to use them and then occasionally when just no semantic element is the correct choice that is the time that we actually should use divs in span so i'm going to delete those for now and save our document and now i'll just scroll our code up to the very top and i'm going to do the same for our page over here on the right now 

## html5 outliner

our current page so we've got our heading hierarchy correct with my goals for the year an untitled nav that's okay we didn't put a heading in there like i said we could have put an h2 it's just saying we didn't have one but a nav doesn't require one but remember if you do have more than one nav element per page then you do need to at least appropriately label that for assistive technology

aside and this aside was inside the second section it's also untitled which is okay and aside does not have to have a heading but it just notes that as it's untitled here if you added a heading inside of the aside say an h4 then it would of course appear


##

how important the headings are the heading hierarchy if you don't get any other semantics correct in your page that's the one thing to really understand is the heading hierarchy of a page but all of these other semantic elements definitely help outline your page and add meaning avoiding these is the biggest mistake you can possibly make as you are constructing an html page okay now that we've looked at our outline 