# Frontend Mentor - Interactive rating component solution


## Table of contents

- [Overview](#overview)
  - [The challenge](#interactive-rating-component)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#html5 #Ccss3 #javascript)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#IrvineMesa #frontendmentor.io)

### Screenshot

![](./component.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process
  For this challenge my process in included using just the three basics of html5, css3, Javascript(ES6).
### Built with

- HTML5
- CSS
- Desktop-first workflow

### What I learned

```
```js
btns.forEach((btn) => {
    btn.addEventListener('click', function (e) {

        // body...
        let selectedBtn = e.currentTarget;
        for (let i = 0; i < btns.length; i++) {
            
            
            if (btns[i].getAttribute('aria-selected') == "true") {
                
                btns[i].setAttribute('aria-selected', false);
                selectedBtn.setAttribute('aria-selected', true);
                selectedRating.textContent = selectedBtn.id;
                
            } else {
                selectedBtn.setAttribute('aria-selected', true);
                selectedRating.textContent = selectedBtn.id;
            }
        }
    });
});
```
### Useful resources

- [w3schools](https://www.w3schools.com/js/js_loop_for.asp) - w3 schools helped me understand the basics of how the for loop is used in javascript and its purpose for selecting buttons etc.

- [youtube](https://www.youtube.com/watch?v=HWWr2WcWiesm) - This is an amazing video done my a gentleman named Irvine Mesa who did a great job explaining the forEach() concept when wanting to select the button ratings for the challenge.



## Author

- Website - [Eric Aguayo](https://www.ericaguayo.com)
- Frontend Mentor - [@EAguayodev](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@EricAguayo13](https://www.twitter.com/yourusername)