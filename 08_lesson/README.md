# HTML 
## TABLE
table to our web page tables structure tabular data that is data that's made up of rows and columns we often see this with schedules statistics in sports and many different types of data flight schedules for example and what we don't want to use tables for are an entire page  layout back in the 90s and early 2000s it was very common to use a table to structure your entire html page so you may see some old code that does that but we do not want to do that we want to stick with semantic html and in the future you'll learn css and we'll design our page layouts with semantic html and css not tables okay tables do really need a little bit of css to look kind of accurate however we can start creating a table without css so let's do that now i'm going to scroll down in our html file and we want to get to this section that says my daily schedule the

## browser dev tools
browser to highlight something that happens here in the code i'm going to right click on the table and click inspect this will open dev tools and it should be showing the elements now if we highlight the table over here in the elements tab in dev tools you can see it's highlighted on the page notice all the orange to the right that is margin that is not table so the table doesn't expand to the width of the page it only expands based on the content inside the table that is different from some other elements like
2:29:45
the paragraph element notice how it expands for the full width of the page or the ordered list element that we have here it expands for the full width of the page the same with the aside element so it's worth noting that the table is different from a lot of other elements that automatically take up the full width of the page the table element only expands to contain the content that is within the table okay

## th

## colspan attribute 
## rowspan attribute

## 
semantics which definitely helps structure a page and tell the browser what the page is about and it also helps assistive technology like screen readers navigate a page
2:32:32
for those that do not use a mouse for example to navigate the page so let's scroll up 

## semantics in table 

### caption 

 caption and we can say what the table is about and that would help someone navigating with the screen reader decide if they really want to navigate the rest of the table or just skip over it and clearly we can also do that visually 

## thead
thead which stands for table head 
it adds semantics to our table

## tbody
t body element for the table body

## tfoot
you could put something in the footer that say totals up all of the columns if you had a ledger that was tracking account numbers or expenses or say you had a sports stats or something like that or anything else that would need totaled up that would be a good place to put it is inside the footer i'm just going to put a statement about our schedule i'm going to scroll up before i add the statement but here i'm just
2:35:06
going to put and that's what i do every day comma five days a week period just eat sleep code and recharge 

footer is spanning both columns and we've clearly defined the semantics for our table 

## rowspan

row span and we came down to this final row and we only added a first and a third column we didn't have to specify that this was the first and this was the third it automatically knew that because the second column in the row above is the one that had the row span of two now

## scope

### scope = col
for each heading that we have on the page each th except this one that has a space in it we need to provide a scope and that says how it relates to the table so this would be scope equals to call which stands for column

### scope = row
i can paste this in but i need to change column to row and i'll copy this and we need to apply this to each one of the row
2:38:41
headings 

## scope and id , header
scope however that you may see that accomplished in another way and that is providing an id for each header 

scope is better than id because we have to apply scope on only head but if we use id after that we have to apply headers on td

## semantics
semantics don't change the look on the page but we have really helped assistive technology navigate our table now this is the easier way to do that with scope 