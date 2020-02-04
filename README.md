# css-sass-htm-complete-guide

Complete reference to css, sass and html

```css
/*
COLORS:

Light green: #7ed56f
Medium green: #55c57a
Dark green: #28b485

*/

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: blanchedalmond;
  font-family: "Lato", sans-serif, Arial, Helvetica, sans-serif;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.7;
  color: #777;
  padding: 30px;
}

/* 
 background-size: cover; //Fit into container irrespective of the view point

*/

.header {
  height: 95vh;
  background-image: linear-gradient(
      to left,
      rgba(25, 153, 8, 0.692),
      rgba(79, 121, 3, 0.562)
    ), url(../img/hero.jpg);
  background-size: cover;
  background-position: top;
  clip-path: polygon(0 0, 100% 0, 100% 75vh, 0% 100%);
  position: relative;
}

.logo-box {
  position: absolute;
  top: 40px;
  left: 40px;
}

.logo {
  height: 35px;
}

.heading-primary {
  color: #fff;
  text-transform: uppercase;
}

.heading-primary-main {
  display: block;
  font-size: 60px;
  font-weight: 400;
  letter-spacing: 20px;
  animation-name: moveInLeft;
  animation-duration: 3s;
  /* animation-delay: 2s; */
  /* animation-iteration-count: 2; */
  /* animation-timing-function: ease-out; */
}

.heading-primary-sub {
  display: block;
  font-size: 20px;
  font-weight: 400;
  letter-spacing: 10px;
}

/* 
translate(-50%, -50%) //Means this is not in relation to the parnt but the element itself
*/
.text-box {
  position: absolute;
  top: 40%;
  left: 50%;
  transform: translate(-50%, -50%);
}

/* CSS ANIMATION 
types

1. Transition
2. 
For better perfomance use 2 properties, opacity and transform in our case

*/

/* CALLING /USING/APPLYING THE ANIMATION

Call this animation in any of your html node you want to apply this animation
2. it needs 2 properties 
a: animation:
b: animation-duration: 3s
*/
@keyframes moveInLeft {
  /* starting */
  /* Make it invisible */
  0% {
    opacity: 0;
    transform: translateX(-100px);
  }

  /* what you want to happen at this point */

  80% {
    transform: translateX(20px);
  }

  /* finish */
  /* Make it visible */
  100% {
    opacity: 1;
  }
}
```
