<!-- headings -->
<!-- # Heading 1 
## gives h2
### gives heading 3 etc -->

# Jade's Website

[![Netlify Status](https://api.netlify.com/api/v1/badges/891e650f-8f94-42fd-863d-191c6c79bc4f/deploy-status)](https://app.netlify.com/sites/jadephipps/deploys)

[LIVE WEBSITE](https://rpssoc.netlify.app/)


We used [this page](https://manparvesh.com/ "web template") for layout inspiration, and I asked Jade to pick out a colour pallete she likes via Color Hunt. She picked [this pallete](https://colorhunt.co/palette/264477 "Color Hunt pallete").

# Issues
I faced several challenges with this project:

## First week
### HTML
Not sure if a `<div>` should go inside the `<nav>` tag or the other way around. I still what tag should go inside which one ~

### CSS
I had a lot of issues with CSS positioning. For example, after creating my nav bar in HTML, I tried to change its `position` property so that it sticks at the top on scroll. I tried changing this property within `header` and within my `.nav-container` class but they messed up the flow: 

```html
 <header>
   <div class="nav-container">
     <a class="nav-name" href="/">Jade Phipps</a>
        <nav>
            <ul>
              <li><a  href="#">.portfolio()</a></li>
            </ul>
          </nav>
        </div>
    </header>
```

```CSS
header{
  position: relative; /* works but doesn't give me the effect I want*/
  position: fixed; /* when used the header's width reduces to half the screen to the left */
}

.nav-container{
  width: 80%;
  margin: 0  auto;
  position: fixed; /* tried it here too but it also messes up layout*/
}
```
From what I read, the `fixed` position takes the element "*out of flow*".

## Second week

I changed the code since after we learned about flexbox I thought it would be easier to use that for my entire layout instead, and it really was! 

I still had issues with `position: fixed;` for my navbar since it doesn't work when using flexbox (I wanted the navbar to scroll/stick to the top as I go down the page). In the end I gave up trying to have that feature haha =)

I  had other issues  with flexbox but I had a meeting with Max and she helped me so much, so lovely and supportive!!! Thank you <3 



