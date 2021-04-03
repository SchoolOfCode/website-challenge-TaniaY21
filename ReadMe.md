<!-- headings -->
<!-- # Heading 1 
## gives h2
### gives heading 3 etc -->

# Jade's Website
We used [this page](https://manparvesh.com/ "web template") for layout inspiration, and I asked Jade to pick out a colour pallete she likes via Color Hunt. She picked [this pallete](https://colorhunt.co/palette/264477 "Color Hunt pallete").

## Issues
I faced several challenges with this project:

### HTML
Not sure if a `<div>` should go inside the `<nav>` tag or the other way around. I still find it confused gridding the layouts and choosing what tag should go inside which one

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
I was unable to find a solution to this problem despite some serious Googling. From what I read, the `fixed` position takes the element "*out of flow*", but I don't know how to fix that. It also led me to the rabbit hole of CSS grid layouts, flexbox, Bootscrap and I got even more confused... I felt like it was overly complicated for something so simple T_T 

I also had issues keeping the `footer` pinned to the very bottom.

