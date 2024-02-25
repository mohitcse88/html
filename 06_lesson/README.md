# HTML

## IMAGE

- html supports multimedia and images are a big part of that

```
<img src="img/html_logo_300x300.jpg" alt="HTML Logo" title="I am Learning HTML5" width="300" height="300" >
```

### /

- image element now notice the image element doesn't have a closing element like we see here with a heading or we see here with a paragraph sometimes you will see it with a slash like that at the end which means it's self closing html does not require that i should say html5 does not require that however if you are using this in the future in something like **react** it may require that so that's just something to be aware of right now i won't put that in because html5 does not require it

### src Attribute

- source attribute tells html where to grab the image
- full relative path to our image it's in the same project here and it's on our local server in this area so we don't need that absolute url that would grab it
- this is once again a relative path to our folder and then to the image

### alt Attribute

- alt attribute has a couple of purposes one is to help assistive technology for those that may not be able to see the image we are putting on the page the assistive technology like a screen reader will read the description of the image so let's put html5 logo as the alt text but this also makes this alt text appear on the page if the image for some reason does not load
- it doesn't find the image and let's see what happens on the page now we have a broken image icon but notice our alt text appears html5 logo so that is another purpose of the alt attribute

### title Attribute

- title now we've seen the title attribute before remember the title text that we provide here in the title attribute is not accessible a screen reader will not read it so this can't be something that is very important that everybody should know this is text that can complement our image but it's not necessarily required the page is complete without it but we can add some complementary text

- it doesn't have to be identical to the alt text at all this should be complementary

- If we mouse over the image we'll see the title pop up

### width and height Attribute

- In the 1990s these were required however for years these have not been required but now they're coming back and it's width and height

- if we put 300 if we just provide the width html will remember or shift the image to match so the aspect ratio stays the same

- good practice to provide height and width both

[User-centric performance metrics By Google](https://web.dev/articles/user-centric-performance-metrics#types_of_metrics)

[Commulative Layout Shift by Google](https://web.dev/articles/cls)

- why it is now recommended to provide the width and the height even though we can change this in the future with css so i'm saying we provide these but yes css may change and override these values so why do we provide them well it's a little complicated but it's called cumulative layout shift if you've ever gone to a web page and you were getting ready to click on something and then you saw the page shift around maybe a pop-up ad appeared or a banner ad and you clicked on something that you didn't intend to click because the button or the image that you wanted to click suddenly moved that is cumulative layout shift
- so we provide the width and the height now to tell the browser hey this is going to take up some space here and this is how much if we don't provide that the browser shifts everything once it figures out the size of the image
- We can still change the size of the image make it responsive which would adapt to mobile devices and everything else with css
- so we really provide this information with the width and the height just to give the browser an idea of the size and the aspect ratio coming in so it just kind of prepares itself and that helps just a little bit it is now **Recommended By Google Developers** that we do provide the width and the height in the image element with our first image added

## Lazy Loading Attribute

```
<img src="img/haridawar.jpg" alt="Haridawar" title="I like t visit haridawar" width="559" height="350" loading="lazy">
```

- we have to **scroll down to see this image** because our page is long enough that if we scroll to the top we don't see our vacation area anymore now this bottom of the page here you could call it a crease if it was a newspaper and a lot of the terminology kind of goes back to newspapers and magazines as we talk about layout and so this bottom part that defines the line that anything below that we do not see right now that's called the fold so anything after this area that we can now see is called below the fold so anything below the fold we have to scroll to see and now we scroll to see this image

- well there's one more attribute for this image that i want to talk about and it's the loading attribute and if we provide loading and we can set it equal to a value and there's two possible values the first one is eager but we never have to provide this this is the value by default so if we do not provide the loading attribute the loading attribute is always there and it's just set to eager we just don't see it

- but the one that we do need to provide is called lazy and what you want to do for performance for your web page is for any image that is below the fold that is one you do not currently see when the page loads you want to set the loading attribute to lazy and that means the browser will only load that image when it knows it is about to show it when we start to scroll now firefox the web browser firefox is much easier to demonstrate this in chrome wants to display the image much earlier so right now this image is close enough to the area that we see

- create some extra space and i can demonstrate

- disable the cache for demonstration because browsers know to save images after they've loaded them initially so they can reload them fast but that is called the **cache** where it stores the images

- reload the page click the reload icon

- we've reloaded and notice down here we just see the html logo file that's all that has loaded right now and now as we scroll down as we get close to the haridawar image file we will see it load because it has the loading attribute set to lazy so only once we get close and we created a lot of space here so we are scrolling down and fairly soon it should pop up there it is we don't see it on the page yet over here but it's getting close so browser loaded it in preparation for us to see it but what that really helps is that it did not load the image right when we loaded our page so that made our page load faster it only loads these images when it thinks it's going to need them and that is lazy loading

- lazy loading technique that helps your pages
  1:47:56
  load faster imagine if you had a page that had a dozen or 20 or even 50 images you wouldn't want the page to continue loading until it loaded all of those images so lazy loading is a very good performance technique especially when you're dealing with lots of images that are below the fold


### figure 

```
<figure>
    <img src="img/haridawar.jpg" alt="Haridawar" title="I like t visit haridawar" width="559"
        height="350" loading="lazy">
    <figcaption>Haridawar is a good place to visit.</figcaption>
</figure>
```

- image indented inside the figure 


- figure with an image and we can add a caption and it tells the browser that the caption big caption element is related to the image which is better than just putting a paragraph

- it the paragraph while we could visually see it's probably related to the image if it was right under the image it's not telling the browser or assistive technology that it is a caption for the image this spells it out for both the browser and assistive technology  

- what we put in here is directly related to this image but it doesn't have to be identical to the alt attribute of the image although it should kind of be a description of the image 

- figure is not just for images 
```
<figure>
    <figcaption>An Example of HTML5 code</figcaption>
    <p>
        <code>&lt;h1&gt;Hello World&lt;/h1&gt;</code>
    </p>
</figure>
```

### figcaption 
- It is the discription of the image or multimedia

- fig caption first the fig caption element needs to either be the first thing inside of a figure or the last thing it can be either

### &lt;code&gt 
- It is a inline element 
- it's a code element code this element code helps you actually display code if that's what you want to use you can use other elements inside of it though so if i want to display html code i can't simply put an h1 element because then it applies this element to the page

### Inspect

```
ctrl + shift + I
```

### br abbreviation 
- break line

### Image Tools

[loremipsum ](https://loremipsum.io/21-of-the-best-placeholder-image-generators/) - image placeholder - 12 of the best placeholder

[unsplash](https://unsplash.com/) - free image resources 

[pexels](https://www.pexels.com/) - free image resources 

[gratisography ](https://gratisography.com/) - free image resources 

[pixabay](https://pixabay.com/) - free image resources 

[irfanview ](https://www.irfanview.com/) - light weight software to edit and resize the image

[canva](https://www.canva.com/) - image editing software 

[tinypng](https://tinypng.com/) - image compreser to make web faster because image size will be small it will bost the performance
