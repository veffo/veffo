![logo](https://github.com/Ashutosh-PMishra/Ashutosh-PMishra/blob/main/Github%20Banner.png)
<h1 align="center">Hi 👋, I'm Ashutosh Mishra</h1>
<h3 align="center">A passionate Software Engineer from India</h3>

<img align="right" alt="coding" width="400" src="https://user-images.githubusercontent.com/55389276/140866485-8fb1c876-9a8f-4d6a-98dc-08c4981eaf70.gif">

<p align="left"> <img src="https://komarev.com/ghpvc/?username=ashutosh-pmishra&label=Profile%20views&color=0e75b6&style=flat" alt="ashutosh-pmishra" /> </p>

- 👨‍💻😅⚡ All of my projects are available at [https://linktr.ee/simplified_learner](https://linktr.ee/simplified_learner)

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://linkedin.com/in/ashutosh mishra" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="ashutosh mishra" height="30" width="40" /></a>
<a href="https://instagram.com/simplified_learner" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="simplified_learner" height="30" width="40" /></a>
<a href="https://www.youtube.com/c/simplified learner" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="simplified learner" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.mathworks.com/" target="_blank" rel="noreferrer"> <img src="https://upload.wikimedia.org/wikipedia/commons/2/21/Matlab_Logo.png" alt="matlab" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://pandas.pydata.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="pandas" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> </p>

<h3 align="left">Support:</h3>


<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=ashutosh-pmishra&show_icons=true&locale=en&layout=compact" alt="ashutosh-pmishra" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=ashutosh-pmishra&show_icons=true&locale=en" alt="ashutosh-pmishra" /></p>












# Fluid Transitions for React Navigation

<a href="https://www.npmjs.com/package/react-navigation-fluid-transitions">
  <img src="https://img.shields.io/npm/v/react-navigation-fluid-transitions.svg?style=flat-square">
</a>
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg"></a>

## Introduction
This project aims to implement a simple yet powerful set of constructs for building fluid transitions between elements when navigating with [React Navigation](https://reactnavigation.org). 

The library is JavaScript only - no linking required.



The library implements a new navigator component called `FluidNavigator` with the same interface and routing configuration as the `StackNavigator`. The library has a component called `Transition` which can be used to build different types of transitions that will automatically be run when navigating between screens using the regular navigation actions.

> The Navigator's API is identical to the StackNavigator except that it does not support a header component. It can easily be integrated with redux and your existing navigation setups.

[Medium article](https://medium.com/@christian.falch/fluid-transitions-with-react-navigation-a049d2f71494)<br/>
[React Native Animation Challenge #1](https://medium.com/@christian.falch/react-native-animation-challenge-1-7022e48a226)

## Installation

To install the library into your project, run yarn or npm:

`yarn add react-navigation-fluid-transitions`

or

`npm i -S react-navigation-fluid-transitions`

> Future improvements and development will be on react-navigation-fluid-transitions@0.3.x.

## Examples
Examples are included in the project and should be runnable from the root of the project folder.

To start the example run the following commands from the terminal:

`npm i` or `yarn`

To start the project run

`react-native run-ios` or `react-native run-android`

### Shared Element Transitions
This example shows how two elements can be set up to automatically transition between each other when navigating between screens. A more detailed edition of this example can be found in the file [SharedElements.js](./Examples/SharedElements.js).

> Note that a shared transition happens between two elements that looks the same. The library animates position and scale between the two hence using different styles and content between the two elements will result in strange transitions.

```javascript
const Screen1 = (props) => (
  <View style={styles.container}>
    <Text>Screen 1</Text>
    <View style={styles.screen1}>
      <Transition shared='circle'>
        <View style={styles.circle}/>
      </Transition>
    </View>
    <Button
      title='Next'
      onPress={() => props.navigation.navigate('screen2')}
    />
  </View>
);

const Screen2 = (props) => (
  <View style={styles.container}>
    <Text>Screen 2</Text>
    <View style={styles.screen2}>
      <Transition shared='circle'>
        <View style={styles.circle2}/>
      </Transition>
    </View>
    <Button
      title='Back'
      onPress={() => props.navigation.goBack()}
    />
  </View>
);

const Navigator = createFluidNavigator({
  screen1: { screen: Screen1 },
  screen2: { screen: Screen2 },
});

```

### Transitions
The library also supports transitions for elements wrapped in the `Transition` component. You can provide appear/disappear transitions that will be animated during navigation.

The `Transition` element supports appear and disappear transitions (appear will be used if disappear is not set), and these can either be one of the predefined transitions - or functions where you provide your own transitions.

```javascript
<Transition appear='scale' disappear='bottom'>
  <View style={styles.circle}/>
</Transition>
```

#### Custom transitions
It is easy to provide custom transitions - just add the transition function to your component's appear or disappear property. The following example creates a transition that will scale in from 88 times the original size of the wrapped component:

```javascript
<Transition appear={myCustomTransitionFunction}>
  <View style={styles.circle}/>
</Transition>

myCustomTransitionFunction = (transitionInfo) => {
  const { progress, start, end } = transitionInfo;
  const scaleInterpolation = progress.interpolate({
    inputRange: [0, start, end, 1],
    outputRange: [88, 80, 1, 1],
  });
  return { transform: [{ scale: scaleInterpolation }] };
}
```

Read more about the parameters and functionality for building [custom transitions](./docs/CustomTransition.md).


















<p align="center">
  <a href="https://codepen.io/aholachek/pen/ERRpEj">
  <img src="./example-assets/rft-logo.gif" width='500px' alt='react-flip-toolkit animated logo' />
  </a>
</p>

[![Minified & Gzipped size](https://badgen.net/bundlephobia/minzip/react-flip-toolkit)](https://bundlephobia.com/result?p=react-flip-toolkit)
[![MIT license](https://badgen.net/npm/license/react-flip-toolkit)](http://opensource.org/licenses/MIT)
[![npm version](https://badgen.net/npm/v/react-flip-toolkit)](https://npmjs.org/package/react-flip-toolkit 'View this project on npm')

**Comparison with other React FLIP libraries**

| Feature                                                                        | [`react-flip-move`](https://github.com/joshwcomeau/react-flip-move) | [`react-overdrive`](https://github.com/berzniz/react-overdrive) | `react-flip-toolkit` |
| ------------------------------------------------------------------------------ | :-----------------------------------------------------------------: | :-------------------------------------------------------------: | :------------------: |
| Animate position                                                               |                                 ✅                                  |                               ✅                                |          ✅          |
| Animate scale                                                                  |                                 ❌                                  |                               ✅                                |          ✅          |
| Animate opacity                                                                |                                 ❌                                  |                               ✅                                |          ✅          |
| [Animate parent's size without warping children](#nested-scale-transforms) |                                 ❌                                  |                               ❌                                |          ✅          |
| Use real FLIP instead of cloning & crossfading                                 |                                 ✅                                  |                               ❌                                |          ✅          |
| [Use springs for animations](https://codesandbox.io/s/react-flip-toolkit-spring-settings-explorer-vjrsh)                                                     |                                 ❌                                  |                               ❌                                |          ✅          |
| Support spring-based stagger effects                                           |                                 ❌                                  |                               ❌                                |          ✅          |
| [Usable with frameworks other than React](packages/flip-toolkit)               |                                 ❌                                  |                               ❌                                |          ✅          |

## Quick start

`npm install react-flip-toolkit` or `yarn add react-flip-toolkit`

1. Wrap all animated children with a single `Flipper` component that has a `flipKey` prop that changes every time animations should happen.

2. Wrap elements that should be animated with `Flipped` components that have a `flipId` prop matching them across renders.


## Table of Contents

- [Forkable Examples](#forkable-examples)
  - [Simple Example: An Expanding Div](#simple-example-an-expanding-div)
  - [Simple Example: Two Divs](#simple-example-two-divs)
  - [Simple Example: List Shuffle](#simple-example-list-shuffle)
  - [List Transitions](#list-transitions)
  - [Stagger Effects](#stagger-effects)
  - [Spring Customizations](#spring-customizations)
  - [Nested Scale Transforms](#nested-scale-transforms)
  - [Route-based Animations With React Router](#route-based-animations-with-react-router)
  - [More examples](#more-examples)
- [The Components](#the-components)
  - [`Flipper`](#flipper)
    - [Basic Props](#basic-props)
    - [Advanced Props](#advanced-props)
  - [`Flipped`](#flipped)
    - [Wrapping a React Component](#wrapping-a-react-component)
    - [Basic props](#basic-props)
    - [Callback props](#callback-props)
    - [Transform props](#transform-props)
    - [Advanced props](#advanced-props)
  - [`Spring`](#spring)
- [Library details](#library-details)
- [Troubleshooting](#troubleshooting)
  - [Problem #1: Nothing is happening](#problem-1-nothing-is-happening)
  - [Problem #2: Things look weird / animations aren't behaving](#problem-2-things-look-weird--animations-arent-behaving)
  - [Problem #3: It's still not working](#problem-3-its-still-not-working)
- [Performance](#performance)
  - [`Memoization`](#memoization)
  - [`will-change:transform`](#will-changetransform)

## Forkable Examples

### Simple Example: An Expanding Div

<a href="https://codesandbox.io/s/8130rn9q2">
<img src="./example-assets/square.gif" height="200px" alt="animated square" />
</a>

[Fork this example on Code Sandbox](https://codesandbox.io/s/8130rn9q2)


```jsx
import React, { useState } from 'react'
import { Flipper, Flipped } from 'react-flip-toolkit'

const AnimatedSquare = () => {
  const [fullScreen, setFullScreen] = useState(false)
  const toggleFullScreen = () => setFullScreen(prevState => !prevState)

  return (
    <Flipper flipKey={fullScreen}>
      <Flipped flipId="square">
        <div
          className={fullScreen ? 'full-screen-square' : 'square'}
          onClick={toggleFullScreen}
        />
      </Flipped>
    </Flipper>
  )
}
```





### List Transitions

Add some interest to a dynamic list of cards by animating changes to cards' sizes and positions.

<a href="https://codesandbox.io/s/list-transitions-ju549">
<img src="./example-assets/listanimations.gif" height="200px" alt='animated list' />
</a>

[Fork this example on Code Sandbox](https://codesandbox.io/s/list-transitions-ju549)

### Stagger Effects

The `react-flip-toolkit` library offers spring-driven stagger configurations so that you can achieve complex sequenced effects.

For the most basic stagger effect, you can simply add a `stagger` boolean prop to your `Flipped` element:

```jsx
<Flipped flipId={`element-${i}`} stagger>
  <AnimatedListItem/>
</Flipped>
```

<a href="https://codesandbox.io/s/wnnxl223n8">
<img src="./example-assets/list-transition.gif" height="300px" alt='animation for the selected state of a list item' />
</a>

[Fork this example on Code Sandbox](https://codesandbox.io/s/wnnxl223n8)


### Spring Customizations

`react-flip-toolkit` uses springs for animations. To customize the spring, you can pass in a preset name:

```jsx
// spring preset can be one of: "stiff", "noWobble", "gentle", "veryGentle", or "wobbly"
<Flipper flipKey='foo' spring='wobbly'>
  {/* Flipped components go here...*/}
</Flipper>
```

or a custom spring config:

```jsx
<Flipper flipKey='foo' spring={{ stiffness: 280, damping: 22 }} >
  {/* Flipped components go here...*/}
</Flipper>
```
[View all spring options in the interactive explorer](https://codesandbox.io/s/react-flip-toolkit-spring-settings-explorer-vjrsh)


### Nested Scale Transforms

<a href="https://codesandbox.io/s/github/aholachek/react-stripe-menu">
<img src="./example-assets/stripe-menu.gif" height="300px" alt="stripe menu" />
</a>

- [Fork this example on Code Sandbox](https://codesandbox.io/s/github/aholachek/react-stripe-menu)
- [Fork Github repo](https://github.com/aholachek/react-stripe-menu)


Interesting animations often involve scale transforms in addition to simple translate transforms. The problem with scale animations has to do with children &mdash; if you scale a div up 2x, you will warp any children it has by scaling them up too, creating a weird-looking animation. That's why this library allows you to wrap the child with a `Flipped` component that has an `inverseFlipId` to counteract the transforms of the parent:

```jsx
<Flipped flipId={id}>
  <div>
    <Flipped inverseFlipId={id} scale>
      <div>some text that will not be warped</div>
    </Flipped>
  </div>
</Flipped>
```

By default, both the scale and the translation transforms of the parent will be counteracted (this allows children components to make their own FLIP animations without being affected by the parent).
But for many use cases, you'll want to additionally specify the `scale` prop to limit the adjustment to the scale and allow the positioning to move with the parent.

Note: the DOM element with the inverse transform should lie flush against its parent container for the most seamless animation.

That means any layout styles &mdash; padding, flexbox, etc&mdash;should be applied to the inverted container (the element wrapped with a `Flipped` component with an `inverseFlipId`) rather than the parent `Flipped` container.



### Route-based Animations With React Router

<a href="https://github.com/aholachek/react-flip-toolkit-router-example">
  <img src="./example-assets/compressed-demo.gif" width='500px' alt='React-flip-toolkit with React-Router' />
</a>

[Fork Github repo](https://github.com/aholachek/react-flip-toolkit-router-example)


`react-flip-toolkit` works great with client-side routers to provide route-driven transitions:

```jsx
<Route
  render={({ location, search }) => {
    return (
      <Flipper
        flipKey={`${location.pathname}-${location.search}`}
      >
      {/* Child routes that contain Flipped components go here...*/}
      </Flipper>
    )
  }}
/>
```

### More examples

- [Guitar shop](https://react-flip-toolkit-demos.surge.sh/guitar)
- [React-flip-toolkit logo](https://codepen.io/aholachek/pen/ERRpEj)
- [Using Portals](https://react-flip-toolkit-demos.surge.sh/portal)

## The Components

### `Flipper`

The parent wrapper component that contains all the elements to be animated. You'll often need only one of these per page, but sometimes it will be more convenient to have multiple `Flipper` regions of your page concerned with different transitions.

```jsx
<Flipper flipKey={someKeyThatChanges}>{/* children */}</Flipper>
```

#### Basic Props

| prop                    |  default   | type                       | details                                                                                                                                                                                                                                                                                                                                                                                                         |
| ----------------------- | :--------: | :------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| flipKey **(required)**  |     -      | `string`, `number`, `bool` | Changing this tells `react-flip-toolkit` to transition child elements wrapped in `Flipped` components.                                                                                                                                                                                                                                                                                                          |
| children **(required)** |     -      | `node`                     | One or more element children                                                                                                                                                                                                                                                                                                                                                                                    |
| spring                  | `noWobble` | `string` or `object`       | Provide a string referencing one of the spring presets &mdash; `noWobble` (default), `veryGentle`, `gentle`, `wobbly`, or `stiff`, OR provide an object with stiffness and damping parameters. [Explore the spring setting options here](https://codesandbox.io/s/react-flip-toolkit-spring-settings-explorer-vjrsh). The prop provided here will be the spring default that can be overrided on a per-element basis on the `Flipped` component. |
| applyTransformOrigin    |   `true`   | `bool`                     | Whether or not `react-flip-toolkit` should apply a transform-origin of "0 0" to animating children (this is generally, but not always, desirable for FLIP animations)                                                                                                                                                                                                                                           |
| element                 |   `div`    | `string`                   | If you'd like the wrapper element created by the `Flipped` container to be something other than a `div`, you can specify that here.                                                                                                                                                                                                                                                                             |
| className               |     -      | `string`                   | A class applied to the wrapper element, helpful for styling.                                                                                                                                                                                                                                                                                                                                                    |
| staggerConfig           |     -      | `object`                   | Provide configuration for staggered `Flipped` children. The config object might look something like the code snippet below:                                                                                                                                                                                                                                                                                     |






### `Flipped`

Wraps an element that should be animated.

E.g. in one component you can have

```jsx
<Flipped flipId="coolDiv">
  <div className="small" />
</Flipped>
```

and in another component somewhere else you can have

```jsx
<Flipped flipId="coolDiv">
  <div className="big" />
</Flipped>
```

and they will be tweened by `react-flip-toolkit`.

The `Flipped` component produces no markup, it simply passes some props down to its wrapped child.

#### Wrapping a React Component

If you want to wrap a React component rather than a JSX element like a `div`, you can provide a render prop and then apply the `flippedProps` directly to the wrapped element in your component:

```jsx
<Flipped>
  {flippedProps => <MyCoolComponent flippedProps={flippedProps} />}
</Flipped>

const MyCoolComponent = ({ flippedProps }) => <div {...flippedProps} />
```

You can also simply provide a regular React component as long as that component spreads unrecognized props directly onto the wrapped element (this technique works well for wrapping styled components):

```jsx
<Flipped>
  <MyCoolComponent />
</Flipped>

const MyCoolComponent = ({ knownProp, ...rest }) => <div {...rest} />
```


#### Transform props

By default the FLIP-ped elements' translate, scale, and opacity properties are all transformed. However, certain effects require more control so if you specify any of these props, _only the specified attribute(s) will be tweened_:

| prop      |  type  | details                             |
| --------- | :----: | :---------------------------------- |
| translate | `bool` | Tween `translateX` and `translateY` |
| scale     | `bool` | Tween `scaleX` and `scaleY`         |
| opacity   | `bool` |                                     |



### `Spring`

As a convenience, `react-flip-toolkit` exports a tiny function to access the same spring system used to create FLIP transitions.

[Fork example on CodeSandbox](https://codesandbox.io/s/react-flip-toolkit-spring-example-e6pyc)

```jsx
import { spring } from 'react-flip-toolkit'

spring({
  config: "wobbly",
  values: {
    translateY: [-15, 0],
    opacity: [0, 1]
  },
  onUpdate: ({ translateY, opacity }) => {
    el.style.opacity = opacity;
    el.style.transform = `translateY(${translateY}px)`;
  },
  delay: i * 25,
  onComplete: () => console.log('done')
});
```

<a href="https://codesandbox.io/s/react-flip-toolkit-spring-example-e6pyc">
  <img src="./example-assets/spring.gif" alt="spring example" width="200px"/>
</a>


## Global configuration functions

You can programmatically call the following functions if you need to disable (or re-enable) FLIP animations everywhere.

#### `disableFlip()`

Global switch to disable all animations in all `Flipper` containers.

#### `enableFlip()`

Global switch to (re-)enable all animations in all `Flipper` containers. Animations are enabled by default. Calling this function is needed only if animations were previously disabled with `disableFlip()`.

#### `isFlipEnabled()`

Returns a boolean indicating whether animations are globally enabled or disabled.


## Library details

<a href="https://www.browserstack.com/">
<img src="./example-assets/browserstack.png" alt="browserstack" width="140"/>
</a>

- Tested in latest Chrome, Firefox, Safari, and Edge with [Browserstack](https://www.browserstack.com/).
- Requires React 16+
- Uses [Rematrix](https://github.com/jlmakes/rematrix) for matrix calculations and a simplified fork of [Rebound](https://github.com/facebook/rebound-js) for spring animations


## Performance

`React-flip-toolkit` does a lot of work under the hood to try to maximize the performance of your animations &mdash; for instance, off-screen elements won't be animated, and style updates are batched to prevent [layout thrashing](https://developers.google.com/web/fundamentals/performance/rendering/avoid-large-complex-layouts-and-layout-thrashing).
However, if you are building particularly complex animations&mdash;ones that involve dozens of elements or large images&mdash; there are some additional strategies you can use to ensure performant animations.



This [CSS property](https://dev.opera.com/articles/css-will-change-property/) tells the browser to anticipate changes to an element. It should be used with caution, because it can increase browser resource usage. If you notice rendering issues in your animation, try seeing if it increases the performance of the animation.



















# Dopefolio 🔥

## A Blazing Fast Multipage Portfolio Template for Developers 🚀

## [Demo Link](https://dopefolio.netlify.app) 🔗

<div align="center">
  <img src="https://i.postimg.cc/CxZXqhWM/ezgif-com-video-to-gif-1.gif" alt="Dopefolio Demo" width="100%" />
  <br>
</div>

<br/>
<br/>

---

<br/>

## ( Update ): Project Achievement 🏆 

**Dopefolio** has been listed as the **Hottest Frontend Tool of 2021** According to **CSS Tricks** 🥳. Thanks to all of you for supporting this project 🙌

**[Link to the CSS tricks article on Dopefolio](https://css-tricks.com/hottest-front-end-tools-in-2021/#aa-58-dopefolio)**   

<br/>

----

<br/>

## Features

- ### **Easy to Setup 💯** 
- ### **Free to Use ( OpenSource ) 🥳** 
- ### **No Additional Frameworks 🤘** 
- ### **No Additional Libraries 🙌** 
- ### **Multi Page 💎** 
- ### **Fully Responsive 🚀** 
- ### **Super Fast and Optimized for SEO ⚡** 
- ### **Great Audits Score 🎖️** 

<img src="https://i.ibb.co/1dD8Mky/Screenshot-from-2021-08-28-14-38-30.png" alt="Dopefolio Audits" width="100%" />

<br/>
<br/>

## Test the template with different colors on the playground link 🚀

## [Playground Link](https://dopefolio-playground.netlify.app) 🔗

<div align="center">
  <img src="https://i.postimg.cc/xjsqN9GG/ezgif-com-gif-maker-2.gif" alt="Dopefolio Playground" width="100%" />
  <br>
</div>

<br/>

----

<br/>

## Technologies used 🛠️

- **HTML** 🚀
- **CSS** 🚀
- **JavaScript** 🚀
- **SASS** 🚀

---

<br/>

## How To Use 🔧

From your command line, first clone Dopefolio:

```bash
# Clone this repository
$ git clone https://github.com/rammcodes/dopefolio

# Go into the repository
$ cd dopefolio

# Remove current origin repository
$ git remote remove origin
```

<br/>

Then you can install the dependencies

Using NPM:

```bash
# Install dependencies
$ npm install

# Listen to changes in CSS Preprocessor files ( SASS files )
$ npm run compile:scss
```

Once you run `npm run compile:scss`, then open the `index.html` inside your favorite browser or using the live server extension.

<br>

---

<br>

## Template Instructions:

## Step 1 - STYLES

Make sure you have started the SASS to CSS compilation by running

```bash
$ npm run compile:scss
```

Change the color theme of the website.

Go to `sass/abstracts/_variables.scss` and change the value of this sass variable called `$themeClrPrimary` to your preferred HEX color.

```scss
// Default value
$themeClrPrimary: #0062b9;
```

**NOTE**: I highly recommend to checkout the [Dopefolio Playground Link](https://dopefolio-playground.netlify.app) to test the template with different colors and see which color do you like the most.

<br/>

---

<br/>

## Step 2 - Homepage



### Projects

- On `.heading-sec__sub`, put a short description about the section.
- `.projects__row` is the row for each project in your portfolio.
- One `.projects__row` for each project in your portfolio ( so for example, if you have 3 projects then you need 3 `.projects__row` one by one).

- Inside each `projects__row`, there are 4 main elements.

  - Project Image is located at `.projects__row-img` where you can add the URL for your project mockup/image. You can use websites like [Media Modifier](https://mediamodifier.com/) and [SmartMockups](https://smartmockups.com) to generate mockups for free. Just make sure to crop the extra white space around your mockup so the mockups can look bigger and the size of the mockup file will be less.

  - `.projects__row-content-title` is where you need to add your Project title.
  - `.projects__row-content-desc` is where you need to add a short 2-3 lines description of your project. As there's going to be a separate page for each project so there you can add all the details for each project on the specific project page.
  - The Anchor tag ( **Case Study** button) on press will take you to the details page for each project ( For example: If you click the **Case Study** button of Project 1 then it will take you to the `project-1.html` file where you will have all the details about that particular project).

Currently, I have already added a separate for each project ( considering there are 3 projects ) the file names are `project-1.html`, `project-2.html`, and `project-3.html`. They all contain the same code only the project title, description and image will change. If you like to add more projects then you can just create a new file for it and paste the same code that we have in `project-1.html` as the code is going to be the same and the only thing that you need to change is the data inside each project.



### Contact Section

- On `.heading-sec__sub`, put a short description about the section.
- `.contact__form-field` is the field inside form. Currently, there are 3 fields but you can add more fields as per your need but just make sure to change the name of **label** and **input/textarea** inside it.

If you like to know how to submit forms so you can receive the form details in your email then highly recommend using **formspree.io** as it's easier to set up and free to use. If you are using **Netlify** to host the site then Netlify has an inbuilt form receiver which you can use instead of **formspree**.





### Footer Section

- Inside h4 tag with the class `heading heading-sm text-lt` add your name.
- On `.main-footer__short-desc` put a short description about yourself.
- On Anchor tag inside `.main-footer__social-cont`, fill the href attribute with a link related to your social media account.



<br/>

---

<br/>



<!-- **** END Project Hero Section **** -->

### Project Details Section

- On `.project-details__showcase-img`, change the value of **src** to the location/link of Project Mockup.
- On `.project-details__desc-para` to add a detailed paragraph describing your project. Use multiple `.project-details__desc-para` elements for multiple paragraphs.
- On `.skills` mention the skills that were used to build the project inside `.skills__skill` to mention each skill.
- On Anchor Tag that says **Live Link** with class `btn btn--med btn--theme project-details__links-btn`, add the Project Live Link as the value for the href attribute.
- On Anchor Tag that says **Code Link** with class `btn btn--med btn--theme-inv project-details__links-btn`, add the Project's Code Link ( Repository Link ) as the value for the href attribute.

<!-- **** Project Details Section **** -->



<!-- **** END Project Details Section **** -->

<br>

---

<br>

---

<br>

## Author 👨‍💻⭐❤️

- **Ram Maheshwari** - **[Linkedin](https://linkedin.com/in/rammcodes)**, **[Instagram](https://instagram.com/rammcodes_)**, **[Twitter](https://twitter.com/rammcodes)**, **[Github](https://github.com/rammcodes)**, **[Portfolio](https://rammaheshwari.com)**  

<br>

#### Note: 
I'm currently looking for good **Job Opportunities** both **Remote ( Worldwide )** and **On-Site ( Anywhere in India )**. So, if you have a good opportunity that matches my skills experience then you can contact me on my **[Linkedin](https://linkedin.com/in/rammcodes)** or my email id **rammcodes@gmail.com** 🙌


<br>

---

<br>

## License 📄

This project is licensed under the  **GPL-3.0** License - see the [LICENSE](LICENSE) file for details


























# 💫 About Me:
👨‍💻 Frontend Web Developer<br>⚡ Tech Content Creator<br>💼 Open To Job Opportunities<br>🌎 rammaheshwari.com <br>


## 🌐 Socials:
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/rammcodes) [![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?logo=Twitter&logoColor=white)](https://twitter.com/rammcodes) [![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/rammcodes_) [![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?logo=YouTube&logoColor=white)](https://youtube.com/@rammcodes) 

# 💻 Tech Stack:
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![SASS](https://img.shields.io/badge/SASS-hotpink.svg?style=for-the-badge&logo=SASS&logoColor=white) ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
# 📊 GitHub Stats:
![](https://github-readme-stats.vercel.app/api?username=rammcodes&theme=dark&hide_border=false&include_all_commits=false&count_private=false)<br/>
![](https://github-readme-streak-stats.herokuapp.com/?user=rammcodes&theme=dark&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=rammcodes&theme=dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

---
[![](https://visitcount.itsvg.in/api?id=rammcodes&icon=0&color=0)](https://visitcount.itsvg.in)

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->


















# Vuedo ![logo](http://i.imgur.com/iBEAx7O.png?2)
[![Build Status](https://travis-ci.org/Vuedo/vuedo.svg?branch=master)](https://travis-ci.org/Vuedo/vuedo) [![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE) [![Join the chat at https://gitter.im/vuedo/Lobby](https://badges.gitter.im/vuedo/Lobby.svg)](https://gitter.im/vuedo/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## What is Vuedo?

Vuedo is an open source project built with Laravel and Vue.js. It is a live example of how everything works together.

Interested in more theory? Here is the [official announcement](https://dotdev.co/announcing-vuedo-an-open-source-project-built-with-laravel-and-vue-js-84f371409401).

## Website using Vuedo in production : [https://vuejsfeed.com/](https://vuejsfeed.com/)

Vue.js Feed is a place where News, Tutorials, Plugins, Showcases and more things regarding Vue are handpicked and shared with the community.

![Dashboard Overview](http://i.imgur.com/4AdbjsF.gif)

## Basic Features:

* Manage posts and media
* Categorize posts
* User Roles
* Content moderation
* Markdown Editor
* Amazon S3 integration
* and more...

## Installation

Download this repo.

Rename `.env.example` to `.env` and fill the options.

Run the following commands:

```
composer install
npm install
php artisan key:generate
php artisan migrate
php artisan db:seed
gulp
php artisan serve
```

If you are making changes to JavaScript or Styles make sure you run `gulp watch`.

## Technical Description

You can find the technical description and a list with the libraries used in development [here](https://github.com/Vuedo/vuedo/wiki/Technical-Description).

## Documentation

Coming soon...

## Issues

For technical questions and bugs feel free to open one issue.

## Contribution

Soon a roadmap for contribution will be added so everyone will be welcome to join.

## Stay In Touch

For latest releases and announcements, follow [@vuedo](https://twitter.com/vuedo) on Twitter.

## License

Vuedo is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).






























# Unity-UI-Rounded-Corners

These components and shaders allow you to add rounded corners to UI elements!


---

![](https://github.com/kirevdokimov/Unity-UI-Rounded-Corners/blob/master/title.gif)

## How to install
### Option 1: Package Manager (Unity 2019.3 and higher)
![](https://github.com/kirevdokimov/Unity-UI-Rounded-Corners/blob/master/how-to-install.gif)
URL to copypaste: 
```
https://github.com/kirevdokimov/Unity-UI-Rounded-Corners.git
```

### Option 2: Package Manager (Manual)
- Open `%projectname%/Packages/manifest.json`
- Add the following to the dependencies section:
```
"com.nobi.roundedcorners": "https://github.com/kirevdokimov/Unity-UI-Rounded-Corners.git"
```

## How to use
#### Symmetrical roundness
- Add `ImageWithRoundedCorners` component to a GameObject with an `Image`
- Adjust `Radius` property
#### Certain roundness value for each corner
- Add `ImageWithIndependentRoundedCorners` to a GameObject with an `Image`
- Adjust `r` Vector4 property. Each vector component represent radius, clockwise, starting with top-left corner
#### Important thing
If you need to add or change the image at runtime, call `Validate()` and then `Refresh()` to update the materials.


# Features
## Changing roundness separately or all at once
![](https://github.com/kirevdokimov/Unity-UI-Rounded-Corners/blob/master/separate-roundness.gif)
## Keeps round while resizing
![](https://github.com/kirevdokimov/Unity-UI-Rounded-Corners/blob/master/gif-01.gif)
## Better quality than sprites
![](https://github.com/kirevdokimov/Unity-UI-Rounded-Corners/blob/master/image-00.png)
## Supports Unity Mask
![](https://github.com/kirevdokimov/Unity-UI-Rounded-Corners/blob/master/gif-02.gif)
## Supports Tint
![](https://github.com/kirevdokimov/Unity-UI-Rounded-Corners/blob/master/gif-04.gif)












![Ah, gl lines](https://cdn.discordapp.com/attachments/377316629220032523/576127655712391198/unknown.png)
# Gizmos
Used for drawing runtime gizmos in builds and editor from any context in the code. It was created when I realized that the built in unity gizmos (Gizmos.DrawWireSphere, etc) don't render in builds, so I made this utility to be able to use.

*Note: Currently doesn't work if a render pipline asset is set in the graphics settings of the project in SRP, if the version of the SRP package is below 7.1.1*

## Requirements
- .NET Framework 4.5
- Git

## Installation
To install for local use, download this repo and copy everything from this repository to `<YourUnityProject>/Packages/Popcron Gizmos` folder.

If using 2018.3.x or higher, you can add a new entry to the manifest.json file in your Packages folder:
```json
"com.popcron.gizmos": "https://github.com/popcron/gizmos.git"
```

The package checks for updates every time a compile happens, and it will say so under the `Popcron/Gizmos/Update` menu if one is available, upon pressing it will make unity update the package to the latest version thats here on github. Though you can always edit it yourself if you'd like. 

## Example
```cs
using UnityEngine;
using Gizmos = Popcron.Gizmos;

[ExecuteAlways]
public class GizmoDrawer : MonoBehaviour
{
    public Material material = null;

    //this will draw in scene view and in game view, in both play mode and edit mode
    private void OnRenderObject()
    {
        //draw a line from the position of the object, to world center
        //with the color green, and dashed as well
        Gizmos.Line(transform.position, Vector3.one, Color.green, true);

        //draw a cube at the position of the object, with the correct rotation and scale
        Gizmos.Cube(transform.position, transform.rotation, transform.lossyScale);
    }

    private void Update()
    {
        //use custom material, if null it uses a default line material
        Gizmos.Material = material;

        //toggle gizmo drawing
        if (Input.GetKeyDown(KeyCode.F3))
        {
            Gizmos.Enabled = !Gizmos.Enabled;
        }
        
        //can also draw from update
        Gizmos.Cone(transform.position, transform.rotation, 15f, 45f, Color.green);
    }
}
```

## Camera render filter
By default, gizmos will only be drawn to the MainCamera, and the Scene view camera. If you'd like to specify other cameras to also render the gizmos, the `Gizmos.CameraFilter` predicate allows you to subscribe to a delegate where you can manually specify if a camera should be rendered to or not.

<details><summary>Example</summary>
<p>
    
```cs
private void OnEnable()
{
    //always sub in on enable, because OnEnable gets called when code gets recompiled AND on awake
    Gizmos.CameraFilter += cam =>
    {
        return cam.name == "MyOtherCamera";
    };
}
```

</p>
</details>

## Custom drawers
The ability to add custom drawers is possible. Inherit from the `Drawer` class and implement the `Draw` method. To see an example of drawing a line using a custom drawer, look at the `LineDrawer.cs` file.

The `Draw` method takes in a ref parameter to a Vector3 array as the buffer, and then a params array of objects. The method expects to return the number of points allocated to the buffer. For example, if renderering a single line, allocate the two points at buffer[0] and buffer[1], and return 2. If the number returned is not the same as the amount of points actually used, then the end result of the drawn element will look incorrect and corrupt.

## API
- `Gizmos.Line` = Draws a line from point a to b. Equivalent to [Gizmos.DrawLine](https://docs.unity3d.com/ScriptReference/Gizmos.DrawLine.html)
- `Gizmos.Square` = Draws a 2D square in the XY plane
- `Gizmos.Cube` = Draws a 3D cube in world space with orientation and scale parameters. Equivalent to [Gizmos.DrawWireCube](https://docs.unity3d.com/ScriptReference/Gizmos.DrawWireCube.html)
- `Gizmos.Bounds` = Draws a representation of a Bounds object
- `Gizmos.Rect` = Draws a rect object to a specific camera
- `Gizmos.Cone` = Draws a cone with specified orientation, length and angle. It looks like the spotlight gizmo
- `Gizmos.Sphere` = Draws a 3D sphere. Equivalent to [Gizmos.DrawWireSphere](https://docs.unity3d.com/ScriptReference/Gizmos.DrawWireSphere.html)
- `Gizmos.Circle` = Draws a 2D circle that is oriented to the camera by default

## Notes
The package uses the same class name as the built-in gizmo class, because of this, you will need to use an alias to point to the right class (`using Gizmos = Popcron.Gizmos`).

The alternative is to make a global class with the same name that redirects all of its calls to Popcron.Gizmos. The downside to this is that you will need to be explicit when calling the UnityEngine.Gizmos class if you ever need to. Choose your poison.

## FAQ
- **What namespace?** 'Popcron'
- **Does it work in builds?** Yes
- **Is there frustum culling?** Yes, it can be toggled with Gizmos.FrustumCulling
- **It's not rendering in game!** Check if your gizmo code is in OnDrawGizmos, because this method isnt called in builds, and ensure that Gizmos.Enabled is true










[![](https://github-readme-stats.vercel.app/api?username=baba-s&hide=contribs&include_all_commits=true&count_private=true&show_icons=true)](https://github.com/anuraghazra/github-readme-stats)
[![](https://github-readme-stats.vercel.app/api/top-langs/?username=baba-s&layout=compact&card_width=100&)](https://github.com/anuraghazra/github-readme-stats)

[![](https://github-profile-trophy.vercel.app/?username=baba-s&rank=-C,-B&margin-w=4)](https://github.com/ryo-ma/github-profile-trophy)

[![](http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=baba-s&theme=github)](https://github.com/vn7n24fzkq/github-profile-summary-cards)

[![](https://github-readme-stats.vercel.app/api/wakatime?username=baba_s&langs_count=10)](https://github.com/anuraghazra/github-readme-stats)

[![](https://skillicons.dev/icons?i=cs,firebase,git,github,jenkins,md,py,rider,unity,vscode,wordpress)](https://skillicons.dev)

[![](https://img.shields.io/twitter/follow/baba_s_?label=Twitter&logo=twitter&style=flat)](https://twitter.com/baba_s_) [![](https://img.shields.io/github/followers/baba-s?label=follow&logo=github&style=flat)](https://github.com/baba-s) [![](https://qiita-badge.apiapi.app/s/baba_s/posts.svg) ](https://qiita.com/baba_s) [![](https://qiita-badge.apiapi.app/s/baba_s/contributions.svg)](https://qiita.com/baba_s)










### Hi there 👋 I'm Ashley Bibizadeh (SimpleTut)

[![](https://vistr.dev/badge?repo=simpletut.simpletut&corners=square)](https://github.com/simpletut/vistr.dev)
[![](https://img.shields.io/badge/-@simpletut-%23181717?style=flat-square&logo=github)](https://github.com/simpletut)

I am a Lead Software Engineer living and working in London (UK) and I am passionate about working with development technologies including Blockchain, Web3, Node JS, React JS, Redux, Apollo and GraphQL.

When I am not working on an Open Source Project I enjoy sharing my knowledge with you, creating premium video tutorials on [My YouTube channel](https://www.youtube.com/c/simpletut) that can help fast track your careers.

## 𝗦𝘁𝗮𝘁𝘀

![simpletut's github stats](https://github-readme-stats.vercel.app/api?username=simpletut&show_icons=true&theme=dracula)


[![Header](https://github.com/AntonioErdeljac/AntonioErdeljac/blob/master/banner.png?raw=true "Header")](https://github.com/AntonioErdeljac)

## 👋 Hello! 
Software engineer with 7+ years of experience.  Worked for innovative startups, large enterprise products, and award-winning agencies.  Familiar with both remote, and in-office roles.  Always seeking to take ownership of the project and deliver faster than expected.  Comfortable for web, mobile, and API development.

## 📚 Writing
Besides developing, I also run a [Youtube Channel](https://www.youtube.com/channel/UCW_4e6sUTMWHxlF06aErH9w).

## 💻 Interesting Contributions
[![Aribnb](https://github-readme-stats.vercel.app/api/pin/?username=airbnb&repo=javascript&theme=dark&show_owner=true)](https://github.com/airbnb/javascript/pull/1693)

## 🛠️ Technologies & Tools
![](https://img.shields.io/badge/Code-JavaScript-informational?style=flat&color=informational&logo=javascript)
![](https://img.shields.io/badge/Code-React-informational?style=flat&color=informational&logo=react)
![](https://img.shields.io/badge/Code-TypeScript-informational?style=flat&color=informational)
![](https://img.shields.io/badge/Code-Vue-informational?style=flat&color=informational&logo=vue.js)
![](https://img.shields.io/badge/Code-EcmaScript-informational?style=flat&color=informational)
![](https://img.shields.io/badge/Code-Node-informational?style=flat&color=informational&logo=node.js)
![](https://img.shields.io/badge/Tool-Webpack-informational?style=flat&color=warning&logo=webpack)
![](https://img.shields.io/badge/Tool-Jest-informational?style=flat&color=warning&logo=jest)
![](https://img.shields.io/badge/Tool-SCSS-informational?style=flat&color=warning&logo=sass)
![](https://img.shields.io/badge/Tool-Docker-informational?style=flat&color=warning&logo=docker)

## 📊 Statistics
[![Antonio's github stats](https://github-readme-stats.vercel.app/api?username=AntonioErdeljac&theme=dark&count_private=true)](https://github.com/anuraghazra/github-readme-stats)

<!--
**AntonioErdeljac/AntonioErdeljac** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->











## Hi there नमस्ते (Namaste)! <img src="https://github.com/inspirasiprogrammer/inspirasiprogrammer/blob/main/wave.gif" width="30px">
<img align="right" alt="GIF" src="https://raw.githubusercontent.com/devSouvik/devSouvik/master/gif3.gif" width="350" style="max-width: 100%;">
<h4> Fullstack web Developer <img src="https://media.giphy.com/media/WUlplcMpOCEmTGBtBW/giphy.gif" width="30"> </h4>
I'm a full-stack web-developer from Kathmandu, Nepal. I graduated in Computer Science and Information Technology from Prime College, Nepal. I like building new stuff and working with other people.


[![Instagram Badge](https://img.shields.io/badge/-@prajwal.iar-purple?style=flat-square&logo=instagram&logoColor=white&link=https://instagram.com/prajwal.iar/)](https://instagram.com/prajwal.iar)
[![Gmail Badge](https://img.shields.io/badge/-prajwal.iar@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:prajwal.iar@gmail.com)](mailto:prajwal.iar@gmail.com)
[![Linkedin Badge](https://img.shields.io/badge/-Prajwalrai-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/prajwal100/)](https://www.linkedin.com/in/prajwal100/)
[![Telegram Badge](https://img.shields.io/badge/-@prajwalrai-0088CC?style=flat&logo=Facebook&logoColor=white)](https://www.facebook.com/Praajwal.iar/ "Contact on Telegram")

Like My Work?

[![Hire Me on Upwork](https://img.shields.io/badge/Hire%20Me%20on-Upwork-brightgreen?logo=upwork&style=for-the-badge)](https://www.upwork.com/freelancers/~01210bb2575a8c05a9)

### You can find my stuff here :leaves:

- My Personal Website :yum: [raiprajwal.com](https://raiprajwal.com)

Here are some ideas to get you started:

- 🔭 I’m currently working on Dimitra Technology
- 🌱 I’m currently learning DevOps
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

## ⚡ Technologies

<!--- just --->

![Laravel](https://img.shields.io/badge/-Laravel-00599C?style=flat-square&logo=Laravel)
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=Node.js&logoColor=white)
![React.js](https://img.shields.io/badge/-React.js-61DAFB?style=flat-square&logo=React&logoColor=white)
![VueJs](https://img.shields.io/badge/vuejs-2.x-brightgreen.svg?style=flat-square)
![JavaScript](https://img.shields.io/badge/-JavaScript-black?style=flat-square&logo=javascript)
![Sequelize](https://img.shields.io/badge/-Sequelize-52B0E7?style=flat-square&logo=Sequelize&logoColor=white)
![TypeORM](https://img.shields.io/badge/-TypeORM-2F323A?style=flat-square&logo=TypeORM&logoColor=white)
![PHP](https://img.shields.io/badge/-PHP-black?style=flat-square&logo=php)
![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3)
![MySQL](https://img.shields.io/badge/-MySQL-black?style=flat-square&logo=mysql)
![Git](https://img.shields.io/badge/-Git-black?style=flat-square&logo=git)
![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github)
![GitLab](https://img.shields.io/badge/-GitLab-FCA121?style=flat-square&logo=gitlab)
![Photoshop](https://img.shields.io/badge/-Photoshop-black?style=flat-square&logo=photoshop)

![Github Stats](https://github-readme-stats.vercel.app/api?username=Prajwal100&count_private=true&show_icons=true&include_all_commits=true)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Prajwal100&hide=TeX&layout=compact)

![Visitor Badge](https://komarev.com/ghpvc/?username=prajwal100&color=green)

### Languages and Tools

<img align="left" src="https://simpleicons.org/icons/laravel.svg" alt="Laravel" height="40px" />
<img align="left" src="https://simpleicons.org/icons/nodedotjs.svg" alt="Node.js" height="40px" />
<img align="left" src="https://simpleicons.org/icons/react.svg" alt="React.js" height="40px" />
<img align="left" src="https://simpleicons.org/icons/sequelize.svg" alt="Sequelize" height="40px" />
<img align="left" src="https://simpleicons.org/icons/html5.svg" alt="HTML5" height="40px" />
<img align="left" src="https://simpleicons.org/icons/css3.svg" alt="CSS3" height="40px" />
<img align="left" src="https://simpleicons.org/icons/visualstudiocode.svg" alt="VSCode" height="40px" />
<img align="left" src="https://simpleicons.org/icons/jetbrains.svg" alt="JetBrains Tools" height="40px" />
<br />

#

<div align="center">

### Show some ❤️ by starring some of the repositories!

</div>















# Project Title

A brief description of what this project does and who it's for


## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 - [Awesome README](https://github.com/matiassingers/awesome-readme)
 - [How to write a Good readme](https://bulldogjob.com/news/449-how-to-write-a-good-readme-for-your-github-project)


## API Reference

#### Get all items

```http
  GET /api/items
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API key |

#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |

#### add(num1, num2)

Takes two numbers and returns the sum.


## Appendix

Any additional information goes here


## Authors

- [@octokatherine](https://www.github.com/octokatherine)


## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)

## Color Reference

| Color             | Hex                                                                |
| ----------------- | ------------------------------------------------------------------ |
| Example Color | ![#0a192f](https://via.placeholder.com/10/0a192f?text=+) #0a192f |
| Example Color | ![#f8f8f8](https://via.placeholder.com/10/f8f8f8?text=+) #f8f8f8 |
| Example Color | ![#00b48a](https://via.placeholder.com/10/00b48a?text=+) #00b48a |
| Example Color | ![#00d1a0](https://via.placeholder.com/10/00b48a?text=+) #00d1a0 |


## Contributing

Contributions are always welcome!

See `contributing.md` for ways to get started.

Please adhere to this project's `code of conduct`.


## Demo

Insert gif or link to demo


## Deployment

To deploy this project run

```bash
  npm run deploy
```


## Documentation

[Documentation](https://linktodocumentation)


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`API_KEY`

`ANOTHER_API_KEY`


## FAQ

#### Question 1

Answer 1

#### Question 2

Answer 2


## Features

- Light/dark mode toggle
- Live previews
- Fullscreen mode
- Cross platform


## Feedback

If you have any feedback, please reach out to us at fake@fake.com


## 🚀 About Me
I'm a full stack developer...


# Hi, I'm Katherine! 👋


## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://katherineoelsner.com/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/)


## Other Common Github Profile Sections
👩‍💻 I'm currently working on...

🧠 I'm currently learning...

👯‍♀️ I'm looking to collaborate on...

🤔 I'm looking for help with...

💬 Ask me about...

📫 How to reach me...

😄 Pronouns...

⚡️ Fun fact...


## 🛠 Skills
Javascript, HTML, CSS...


## Installation

Install my-project with npm

```bash
  npm install my-project
  cd my-project
```
    
## Lessons Learned

What did you learn while building this project? What challenges did you face and how did you overcome them?


## License

[MIT](https://choosealicense.com/licenses/mit/)


![Logo](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/th5xamgrr6se0x5ro4g6.png)


## Optimizations

What optimizations did you make in your code? E.g. refactors, performance improvements, accessibility


## Related

Here are some related projects

[Awesome README](https://github.com/matiassingers/awesome-readme)


## Roadmap

- Additional browser support

- Add more integrations


## Run Locally

Clone the project

```bash
  git clone https://link-to-project
```

Go to the project directory

```bash
  cd my-project
```

Install dependencies

```bash
  npm install
```

Start the server

```bash
  npm run start
```


## Screenshots

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)


## Support

For support, email fake@fake.com or join our Slack channel.


## Tech Stack

**Client:** React, Redux, TailwindCSS

**Server:** Node, Express


## Running Tests

To run tests, run the following command

```bash
  npm run test
```


## Usage/Examples

```javascript
import Component from 'my-project'

function App() {
  return <Component />
}
```


## Used By

This project is used by the following companies:

- Company 1
- Company 2





















[![MasterHead](https://firebasestorage.googleapis.com/v0/b/flexi-coding.appspot.com/o/dempgi7-520f8d5f-63d4-4453-8822-dbc149ae27f8.gif?alt=media&token=91c0c7b2-93c3-4029-b011-1a8703c5730d)](https://rishavchanda.io)
<h1 align="center">Hi 👋, I'm Rishav Chanda</h1>
<h3 align="center">A passionate FullStack Developer from India</h3>
<img align="right" alt="Coding" width="400" src="https://cdn.dribbble.com/users/1162077/screenshots/3848914/programmer.gif">


<p align="left"> <img src="https://komarev.com/ghpvc/?username=rishavchanda&label=Profile%20views&color=0e75b6&style=flat" alt="rishavchanda" /> </p>

<p align="left"> <a href="https://twitter.com/rishavchanda" target="blank"><img src="https://img.shields.io/twitter/follow/rishavchanda?logo=twitter&style=for-the-badge" alt="rishavchanda"  </p>

- 🔭 I’m currently working on **Vexa Web App**

- 🌱 I’m currently learning **DevOps**

- 💬 Ask me about **Android , MEARN**

- 📫 How to reach me **rishavchanda0@gmail.com**

- ⚡ Fun fact **I am Funny**

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://twitter.com/rishavchanda" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="rishavchanda" height="30" width="40" /></a>
<a href="https://linkedin.com/in/rishav-chanda-b89a791b3" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="rishav-chanda-b89a791b3" height="30" width="40" /></a>
<a href="https://instagram.com/rishav_chanda" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="rishav_chanda" height="30" width="40" /></a>
<a href="https://www.youtube.com/c/rishav chanda" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="rishav chanda" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://aws.amazon.com/amplify/" target="_blank" rel="noreferrer"> <img src="https://docs.amplify.aws/assets/logo-dark.svg" alt="amplify" width="40" height="40"/> </a> <a href="https://developer.android.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/android/android-original-wordmark.svg" alt="android" width="40" height="40"/> </a> <a href="https://angular.io" target="_blank" rel="noreferrer"> <img src="https://angular.io/assets/images/logos/angular/angular.svg" alt="angular" width="40" height="40"/> </a> <a href="https://angular.io" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/angularjs/angularjs-original-wordmark.svg" alt="angularjs" width="40" height="40"/> </a> <a href="https://www.arduino.cc/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/arduino-1.svg" alt="arduino" width="40" height="40"/> </a> <a href="https://getbootstrap.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bootstrap/bootstrap-plain-wordmark.svg" alt="bootstrap" width="40" height="40"/> </a> <a href="https://www.cprogramming.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="c" width="40" height="40"/> </a> <a href="https://www.w3schools.com/cpp/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> </a> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://dart.dev" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/dartlang/dartlang-icon.svg" alt="dart" width="40" height="40"/> </a> <a href="https://www.docker.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="docker" width="40" height="40"/> </a> <a href="https://expressjs.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original-wordmark.svg" alt="express" width="40" height="40"/> </a> <a href="https://www.figma.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/figma/figma-icon.svg" alt="figma" width="40" height="40"/> </a> <a href="https://firebase.google.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" alt="firebase" width="40" height="40"/> </a> <a href="https://flutter.dev" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/flutterio/flutterio-icon.svg" alt="flutter" width="40" height="40"/> </a> <a href="https://cloud.google.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/google_cloud/google_cloud-icon.svg" alt="gcp" width="40" height="40"/> </a> <a href="https://git-scm.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="git" width="40" height="40"/> </a> <a href="https://graphql.org" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/graphql/graphql-icon.svg" alt="graphql" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.adobe.com/in/products/illustrator.html" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/adobe_illustrator/adobe_illustrator-icon.svg" alt="illustrator" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://kotlinlang.org" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/kotlinlang/kotlinlang-icon.svg" alt="kotlin" width="40" height="40"/> </a> <a href="https://www.linux.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/> </a> <a href="https://www.mongodb.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="mongodb" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://nextjs.org/" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/nextjs-2.svg" alt="nextjs" width="40" height="40"/> </a> <a href="https://nodejs.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="nodejs" width="40" height="40"/> </a> <a href="https://opencv.org/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/opencv/opencv-icon.svg" alt="opencv" width="40" height="40"/> </a> <a href="https://postman.com" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" alt="postman" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> <a href="https://reactnative.dev/" target="_blank" rel="noreferrer"> <img src="https://reactnative.dev/img/header_logo.svg" alt="reactnative" width="40" height="40"/> </a> <a href="https://redux.js.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redux/redux-original.svg" alt="redux" width="40" height="40"/> </a> <a href="https://tailwindcss.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tailwindcss/tailwindcss-icon.svg" alt="tailwind" width="40" height="40"/> </a> <a href="https://www.tensorflow.org" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/tensorflow/tensorflow-icon.svg" alt="tensorflow" width="40" height="40"/> </a> <a href="https://unity.com/" target="_blank" rel="noreferrer"> <img src="https://www.vectorlogo.zone/logos/unity3d/unity3d-icon.svg" alt="unity" width="40" height="40"/> </a> <a href="https://www.adobe.com/products/xd.html" target="_blank" rel="noreferrer"> <img src="https://cdn.worldvectorlogo.com/logos/adobe-xd.svg" alt="xd" width="40" height="40"/> </a> </p>

[![Sarthak's GitHub activity graph](https://activity-graph.herokuapp.com/graph?username=rishavchanda&&theme=xcode)](https://github.com/rishavchanda)

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=rishavchanda&show_icons=true&locale=en&layout=compact&theme=tokyonight" alt="rishavchanda" /></p>

<p>&nbsp;<img align="center" src="https://github-readme-stats.vercel.app/api?username=rishavchanda&show_icons=true&locale=en&theme=tokyonight" alt="rishavchanda" /></p>

<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=rishavchanda&&theme=tokyonight" alt="rishavchanda" /></p>























![banner](https://user-images.githubusercontent.com/70807684/155843098-4a8190e2-daf9-4811-8e6a-f698ff7039f0.gif)

  <h3 align= "center"> Hello World 👋🏼 It's Avid Coder 💓 </h3>

----

 Here's some fun facts about me:

- I hope to pursue a career in web development one day (but for now, I stick to open-source contributions 😀)
- Although I code, my main career focus is to work in medical science 🧪🔬
- I love football (soccer) ⚽
- I created [the CodingContributorsLair Organization](https://github.com/CodingContributorsLair/) and am part of so many more organisations!

-----

My Github stats:

<table>
    <tr>
        <td>
            <img src="https://github-readme-streak-stats.herokuapp.com/?user=AvidCoder101&theme=radical"/>
        </td>
        <td>
            <img src="https://github-profile-trophy.vercel.app/?username=AvidCoder101"/>
        </td>
    </tr>
    <tr>
        <td>
            <img src="https://github-readme-stats.vercel.app/api?username=avidcoder101&count_private=true&show_icons=true&theme=radical"/>
        </td>
        <td>
            <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=avidcoder101&langs_count=10&layout=compact&hide=php,batchfile,gherkin,freemarker,xslt,tsql,ruby"/>
        </td>
    </tr>
</table>

----

Organisations I am part of:

[<img src= "https://avatars.githubusercontent.com/u/66388388?s=88&v=4" height= "50" width= "50">](https://github.com/EddieHubCommunity)
[<img src= "https://avatars.githubusercontent.com/u/35373879?s=60&v=4" height= "50" width= "50">](https://github.com/zero-to-mastery)
[<img src= "https://avatars.githubusercontent.com/u/87652881?s=200&v=4" height= "50" width= "50">](https://github.com/CodingContributorsLair)
[<img src= "https://avatars.githubusercontent.com/u/67384272?s=88&v=4" height= "50" width= "50">](https://github.com/MakeContributions)
[<img src= "https://avatars.githubusercontent.com/u/37713493?s=88&v=4" height= "50" width= "50">](https://github.com/firstcontributions)
[<img src= "https://avatars.githubusercontent.com/u/24355438?s=88&v=4" height= "50" width= "50">](https://github.com/fnplus)
[<img src= "https://avatars.githubusercontent.com/u/68013560?s=88&v=4" height= "50" width= "50">](https://github.com/jobream)
[<img src= "https://avatars.githubusercontent.com/u/88003901?s=60&v=4" height= "50" width= "50">](https://github.com/App-Choreography)
[<img src= "https://avatars.githubusercontent.com/u/78741698?s=60&v=4" height= "50" width= "50">](https://github.com/chryz-hub)
[<img src= "https://avatars.githubusercontent.com/u/55499010?s=60&v=4" height= "50" width= "50">](https://github.com/devcreatives)
[<img src= "https://avatars.githubusercontent.com/u/69833530?s=60&v=4" height= "50" width= "50">](https://github.com/uncodedtech)
[<img src= "https://avatars.githubusercontent.com/u/70080194?s=64&v=4" height= "50" width= "50">](https://github.com/golang-friends)
[<img src= "https://avatars.githubusercontent.com/u/72601117?s=200&v=4" height= "50" width= "50">](https://github.com/nit-ap)
[<img src= "https://avatars.githubusercontent.com/u/72855943?s=88&v=4" height= "50" width= "50">](https://github.com/CodeAvailable)
[<img src= "https://avatars.githubusercontent.com/u/75231084?s=88&v=4" height= "50" width= "50">](https://github.com/RoquesBeach)
[<img src= "https://avatars.githubusercontent.com/u/85593293?s=200&v=4" height= "50" width= "50">](https://github.com/64-shades)
[<img src= "https://avatars.githubusercontent.com/u/81645243?s=64&v=4" height= "50" width= "50">](https://github.com/nhcommunity)
[<img src= "https://avatars.githubusercontent.com/u/97304647?s=64&v=4" height= "50" width= "50">](https://github.com/Intel-Student-Ambassadors)
[<img src= "https://avatars.githubusercontent.com/u/95956083?s=64&v=4" height= "50" width= "50">](https://github.com/InnateComm)
[<img src= "https://avatars.githubusercontent.com/u/95483713?s=64&v=4" height= "50" width= "50">](https://github.com/CommunityPro)
[<img src= "https://avatars.githubusercontent.com/u/90423790?s=64&v=4" height= "50" width= "50">](https://github.com/Robotics-Club-BMU)
[<img src= "https://avatars.githubusercontent.com/u/86231837?s=200&v=4" height= "50" width= "50">](https://github.com/OSCA-Kampala-Chapter)
[<img src= "https://avatars.githubusercontent.com/u/90124840?s=64&v=4" height= "50" width= "50">](https://github.com/Bauddhik-Geeks)
[<img src= "https://avatars.githubusercontent.com/u/88617467?s=64&v=4" height= "50" width= "50">](https://github.com/OpInCo-Community)
[<img src= "https://avatars.githubusercontent.com/u/86716722?s=64&v=4" height= "50" width= "50">](https://github.com/CURAJ-Open-Source-Community)
[<img src= "https://avatars.githubusercontent.com/u/83757303?s=64&v=4" height= "50" width= "50">](https://github.com/CuriousGrids)
[<img src= "https://avatars.githubusercontent.com/u/37249458?s=64&v=4" height= "50" width= "50">](https://github.com/risk-first)
[<img src= "https://avatars.githubusercontent.com/u/83161372?s=200&v=4" height= "50" width= "50">](https://github.com/devstrons)
[<img src= "https://avatars.githubusercontent.com/u/92242633?s=200&v=4" height= "50" width= "50">](https://github.com/websycode)
[<img src= "https://avatars.githubusercontent.com/u/95528872?s=200&v=4" height= "50" width= "50">](https://github.com/Magic-Academy)
[<img src= "https://avatars.githubusercontent.com/u/83478816?s=200&v=4" height= "50" width= "50">](https://github.com/Design-and-Code)
[<img src= "https://avatars.githubusercontent.com/u/107547777?s=200&v=4" height= "50" width= "50">](https://github.com/AccessibleForAll)
[<img src= "https://avatars.githubusercontent.com/u/105087028?s=200&v=4" height= "50" width= "50">](https://github.com/infraform)
[<img src= "https://avatars.githubusercontent.com/u/99540144?s=200&v=4" height= "50" width= "50">](https://github.com/devs-in-tech)
[<img src= "https://avatars.githubusercontent.com/u/88209946?s=200&v=4" height= "50" width= "50">](https://github.com/The-CODE-Plus-Plus-Community)
[<img src= "https://avatars.githubusercontent.com/u/99627011?s=200&v=4" height= "50" width= "50">](https://github.com/Huniko-Team)

---

Languages I know:

![](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![](https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white)
![](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)

---

Some of my repositories:

- **[My Profile Repo - AvidCoder101/AvidCoder101](https://github.com/AvidCoder101/AvidCoder101)**
- **[My BMI Calculator Repo - AvidCoder101/BMICalculator](https://github.com/AvidCoder101/BMICalculator)**
- **[My To-do List Repo - AvidCoder101/To-do-list](https://github.com/AvidCoder101/To-do-list)**
- **[My Harry Potter Quiz Repo - AvidCoder101/Harry-Potter-Quiz](https://github.com/AvidCoder101/Harry-Potter-Quiz)**
- **[My Drawing Repo - AvidCoder101/Drawing-App](https://github.com/AvidCoder101/Drawing-App)**
- **[My Clock Repo - AvidCoder101/Clock-App](https://github.com/AvidCoder101/Clock-App)**

---

 My Codewars Stats:

<img src= "https://www.codewars.com/users/edu_Itis/badges/micro" width= "200"/>

---

Thanks for visiting! Feel free to fork and ⭐ this repo </h3>








































<!--🌯GITHUBWRAPPED / 🌐WEBSITE: https://github.com/neat-run/wrapped -->
<!--<p align="center"> -->
<!--<a href="https://trinib.wrapped.run"><b>My GitHub Wrapped</b></a> -->

<!--🌯GITHUBTERMINALSTATS💻 / 🌐WEBSITE: https://github.com/yogeshwaran01/github-stats-terminal-style -->
<p align="center">
<img src="https://raw.githubusercontent.com/trinib/github-stats-terminal-style/master/github_stats.svg">

<!--📊STATSGRAPH / 🌐WEBSITE: https://github.com/anuraghazra/github-readme-stats -->
<p align="center">
<img src="https://github-readme-stats-trinibs-projects.vercel.app/api?username=trinib&show_icons=true&theme=merko&border_color=599200">

<!--📊STREAKSTATSGRAPH / 🌐WEBSITE: https://github.com/denvercoder1/github-readme-streak-stats -->
<img src="https://github-readme-streak-stats-trinibs-projects.vercel.app/?user=trinib&theme=merko&border=599200">

<!--📙LANGUAGES / 🌐WEBSITE: https://github.com/anuraghazra/github-readme-stats -->
<p align="center">
<a href="https://github.com/trinib/AdGuard-WireGuard-Unbound-DNScrypt"><img src="https://github-readme-stats-trinibs-projects.vercel.app/api/top-langs?username=trinib&theme=merko&layout=compact&border_color=599200&langs_count=6">

<!--✨REPO / 🌐WEBSITE: https://github.com/anuraghazra/github-readme-stats -->
<img src="https://github-readme-stats-trinibs-projects.vercel.app/api/pin/?username=trinib&repo=AdGuard-WireGuard-Unbound-DNScrypt&theme=merko&border_color=599200">

<!--🏆TROPHY / 🌐WEBSITE: https://github.com/ryo-ma/github-profile-trophy -->
<div align="center">
<img src="https://github-profile-trophy-trinibs-projects.vercel.app/?username=trinib&theme=matrix&no-bg=true&no-frame=true&row=1&column=4&title=MultiLanguage,Commits,Followers,PullRequest">
 </div>

<div align="center">
<img src="https://github-profile-trophy-trinibs-projects.vercel.app/?username=trinib&theme=matrix&no-bg=true&no-frame=true&row=1&column=4&title=Repositories,Issues,Organizations,Stars">
 </div>

<!--👨‍💻STACKOVERFLOW / 🌐WEBSITE: https://github.com/omidnikrah/github-readme-stackoverflow -->
<p align="center">
<a href="https://stackoverflow.com/users/14602915/trinib?tab=profile"><img src="https://github-readme-stackoverflow-trinibs-projects.vercel.app/?userID=14602915&theme=dark">
  
<!--📛BADGES / 🌐WEBSITE: https://github.com/DenverCoder1/custom-icon-badges && https://github.com/idealclover/GitHub-Star-Counter -->
<p align="center">
  <a href="https://github.com/trinib?tab=stars&sort=stargazers">
    <img alt="total stars" title="Total stars on GitHub" src="https://custom-icon-badges.demolab.com/badge/dynamic/json?logo=star&color=55960c&labelColor=488207&label=Stars&style=for-the-badge&query=%24.stars&url=https://api.github-star-counter.workers.dev/user/trinib"/></a>
<a href="https://github.com/trinib?tab=followers">
    <img alt="followers" title="Follow me on Github" src="https://custom-icon-badges.herokuapp.com/github/followers/trinib?color=23960c&labelColor=188207&style=for-the-badge&logo=person-add&label=Followers&logoColor=white"/></a>

<!--👀VIEWS / 🌐WEBSITE: https://github.com/antonkomarev/github-profile-views-counter -->
<p align="center">
<img src="https://komarev.com/ghpvc/?username=trinib&color=0E9C47&style=for-the-badge">







<!--📉METRICS / 🌐WEBSITE: https://github.com/lowlighter/metrics -->
<h4 align="right">
<details><summary><b>𝓟&nbsp;𝓡&nbsp;𝓞&nbsp;𝓕&nbsp;𝓘&nbsp;𝓛&nbsp;𝓔&nbsp;&nbsp; 𝓜&nbsp;𝓔&nbsp;𝓣&nbsp;𝓡&nbsp;𝓘&nbsp;𝓒&nbsp;𝓢<img src="https://media.giphy.com/media/mBYkXvLxkHZFmqBHIC/giphy.gif" width=50px height=40px></b></summary>
<p>
<p align="center">
<img src="https://raw.githubusercontent.com/trinib/trinib/main/github-metrics.svg">
</p>
</details>









      
#
<!--✏️WORDBOARD / 🌐WEBSITE: https://github.com/JessicaLim8/JessicaLim8 --> 
<h2 align="center">
Join the Word Cloud Board :cloud: :pencil2:

### :thought_balloon: <a href="https://github.com/trinib/word-cloud/issues/new?template=addword.md&title=wordcloud%7Cadd%7C%3CINSERT-WORD%3E"><b>Add your name</b></a> to see the word cloud update in real time :rocket:

:star2: Don't like the arrangement? <a href="https://github.com/trinib/word-cloud/issues/new?template=shufflecloud.md&title=wordcloud%7Cshuffle"><b>Regenerate it</b></a> :game_die:

<h3 align="center">
📛Github Usernames📛 
</br> 







<!--🖼️🖼️INTERSTLOGOS-->
<p align="center">
<img src="https://www.vectorlogo.zone/logos/flutterio/flutterio-icon.svg" width="60">
<img src="https://www.vectorlogo.zone/logos/python/python-icon.svg" width="60">
<img src="https://www.vectorlogo.zone/logos/firebase/firebase-icon.svg" width="60">
<img src="https://www.vectorlogo.zone/logos/dartlang/dartlang-icon.svg" width="60">
<img src="https://www.vectorlogo.zone/logos/adobe_illustrator/adobe_illustrator-icon.svg" width="60">
<img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/visual-studio-code/visual-studio-code.png" width="60">
<img src="https://www.vectorlogo.zone/logos/linux/linux-icon.svg" width="60">
<img src="https://www.vectorlogo.zone/logos/android/android-icon.svg" width="60">
<img src="https://www.vectorlogo.zone/logos/microsoft/microsoft-icon.svg" width="60">
<img src="https://www.vectorlogo.zone/logos/github/github-icon.svg" width="60">
</h4>


 



 

 



























# Gatsby + Netlify CMS Starter

[![Netlify Status](https://api.netlify.com/api/v1/badges/b654c94e-08a6-4b79-b443-7837581b1d8d/deploy-status)](https://app.netlify.com/sites/gatsby-starter-netlify-cms-ci/deploys)

**Note:** This starter uses [Gatsby v4](https://www.gatsbyjs.com/gatsby-4/).

This repo contains an example business website that is built with [Gatsby](https://www.gatsbyjs.org/), and [Netlify CMS](https://www.netlifycms.org): **[Demo Link](https://gatsby-netlify-cms.netlify.com/)**.

It follows the [JAMstack architecture](https://jamstack.org) by using Git as a single source of truth, and [Netlify](https://www.netlify.com) for continuous deployment, and CDN distribution.

## Features

- A simple landing page with blog functionality built with Netlify CMS
- Editable Pages: Landing, About, Product, Blog-Collection and Contact page with Netlify Form support
- Create Blog posts from Netlify CMS
- Tags: Separate page for posts under each tag
- Basic directory organization
- Uses Bulma for styling, but size is reduced by `gatsy-plugin-purgecss`
- Blazing fast loading times thanks to pre-rendered HTML and automatic chunk loading of JS files
- Uses `gatsby-plugin-image` with Netlify-CMS preview support
- Separate components for everything
- Netlify deploy configuration
- Netlify function support, see `netlify/functions` folder
- Perfect score on Lighthouse for SEO, Accessibility and Performance (wip:PWA)
- ..and more

## Prerequisites

- Minimal Node.js version 14.15.0
- [Gatsby CLI](https://www.gatsbyjs.com/docs/reference/gatsby-cli/)
- [Netlify CLI](https://github.com/netlify/cli)

## Getting Started (Recommended)

Netlify CMS can run in any frontend web environment, but the quickest way to try it out is by running it on a pre-configured starter site with Netlify. The example here is the Kaldi coffee company template (adapted from [One Click Hugo CMS](https://github.com/netlify-templates/one-click-hugo-cms)). Use the button below to build and deploy your own copy of the repository:

<a href="https://app.netlify.com/start/deploy?repository=https://github.com/netlify-templates/gatsby-starter-netlify-cms&amp;stack=cms"><img src="https://www.netlify.com/img/deploy/button.svg" alt="Deploy to Netlify"></a>

After clicking that button, you’ll authenticate with GitHub and choose a repository name. Netlify will then automatically create a repository in your GitHub account with a copy of the files from the template. Next, it will build and deploy the new site on Netlify, bringing you to the site dashboard when the build is complete. Next, you’ll need to set up Netlify’s Identity service to authorize users to log in to the CMS.

### Access Locally

Pulldown a local copy of the Github repository Netlify created for you, with the name you specified in the previous step

```
$ git clone https://github.com/[GITHUB_USERNAME]/[REPO_NAME].git
$ cd [REPO_NAME]
$ yarn
$ netlify dev # or ntl dev
```

This uses [Netlify Dev](https://www.netlify.com/products/dev/?utm_source=blog&utm_medium=netlifycms&utm_campaign=devex) CLI feature to serve any functions you have in the `netlify/functions` folder.

To test the CMS locally, you'll need to run a production build of the site:

```
$ npm run build
$ netlify dev # or ntl dev
```

### Media Libraries (installed, but optional)

Media Libraries have been included in this starter as a default. If you are not planning to use `Uploadcare` or `Cloudinary` in your project, you **can** remove them from module import and registration in `src/cms/cms.js`. Here is an example of the lines to comment or remove them your project.

```javascript
import CMS from "netlify-cms-app";
// import uploadcare from 'netlify-cms-media-library-uploadcare'
// import cloudinary from 'netlify-cms-media-library-cloudinary'

import AboutPagePreview from "./preview-templates/AboutPagePreview";
import BlogPostPreview from "./preview-templates/BlogPostPreview";
import ProductPagePreview from "./preview-templates/ProductPagePreview";
import IndexPagePreview from "./preview-templates/IndexPagePreview";

// CMS.registerMediaLibrary(uploadcare);
// CMS.registerMediaLibrary(cloudinary);

CMS.registerPreviewTemplate("index", IndexPagePreview);
CMS.registerPreviewTemplate("about", AboutPagePreview);
CMS.registerPreviewTemplate("products", ProductPagePreview);
CMS.registerPreviewTemplate("blog", BlogPostPreview);
```

Note: Don't forget to also remove them from `package.json` and `yarn.lock` / `package-lock.json` using `yarn` or `npm`. During the build netlify-cms-app will bundle the media libraries as well, having them removed will save you build time.
Example:

```
yarn remove netlify-cms-media-library-uploadcare
```

OR

```
yarn remove netlify-cms-media-library-cloudinary
```

## Getting Started (Without Netlify)

```
$ gatsby new [SITE_DIRECTORY_NAME] https://github.com/netlify-templates/gatsby-starter-netlify-cms/
$ cd [SITE_DIRECTORY_NAME]
$ npm run build
$ npm run start
```

### Setting up the CMS

Follow the [Netlify CMS Quick Start Guide](https://www.netlifycms.org/docs/quick-start/#authentication) to set up authentication, and hosting for production.

If you want use Netlify CMS locally, run the site in one terminal with `npm run start` and in another
Terminal you can use `npx netlify-cms-proxy-server` which proxy requests so you'll be automatically logged
in as a user on [http:localhost:3000/admin](http:localhost:3000/admin).

## Debugging

Windows users, who aren't using [WSL](https://docs.microsoft.com/en-us/windows/wsl/about), might encounter `node-gyp` errors when trying to npm install.
To resolve, make sure that you have both Python 2.7 and the Visual C++ build environment installed.

```
npm config set python python2.7
npm install --global --production windows-build-tools
```

[Full details here](https://www.npmjs.com/package/node-gyp "NPM node-gyp page").

MacOS and WSL users who might also encounter some errors, check [node-gyp](https://github.com/nodejs/node-gyp) for more info. We recommend using the latest stable node version.

## Purgecss

This plugin uses [gatsby-plugin-purgecss](https://www.gatsbyjs.org/packages/gatsby-plugin-purgecss/) and [bulma](https://bulma.io/). The bulma builds are usually ~170K but reduced 90% by purgecss.

# CONTRIBUTING

Contributions are always welcome, no matter how large or small. Before contributing,
please read the [code of conduct](CODE_OF_CONDUCT.md).





































<p align="center">
<a href="https://www.linkedin.com/in/kakbar"><img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"></a>
</p>

<p align="center"><img src="https://komarev.com/ghpvc/?username=kakbar&style=flat-square&color=blue" alt=""></p>

<h1 align="center">hey there <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="40"></h1>



### :woman_technologist: &nbsp;About Me :

I am a Full Stack Developer <img src="https://media.giphy.com/media/WUlplcMpOCEmTGBtBW/giphy.gif" width="30"> from India.

- 🔭 I’m working as a Software Engineer and contributing to frontend and backend for building web applications.
- 🌱 Exploring Technical Content Writing.
- ⚡ In my free time I solve problems on GeeksforGeeks and read tech articles.
- 📫 How to reach me: &nbsp; [![Linkedin Badge](https://img.shields.io/badge/-kakbar-blue?style=flat&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/kakbar)

---

### 🛠 &nbsp;Languages and Tools :

<p>
<img src="https://github.com/devicons/devicon/blob/master/icons/java/java-original-wordmark.svg" title="Java" alt="Java" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/react/react-original-wordmark.svg" title="React" alt="React" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/spring/spring-original-wordmark.svg" title="Spring" alt="Spring" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/materialui/materialui-original.svg" title="Material UI" alt="Material UI" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/flutter/flutter-original.svg" title="Flutter" alt="Flutter" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/redux/redux-original.svg" title="Redux" alt="Redux " width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/css3/css3-plain-wordmark.svg"  title="CSS3" alt="CSS" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/html5/html5-original.svg" title="HTML5" alt="HTML" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/javascript/javascript-original.svg" title="JavaScript" alt="JavaScript" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/firebase/firebase-plain-wordmark.svg" title="Firebase" alt="Firebase" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/gatsby/gatsby-original.svg" title="Gatsby"  alt="Gatsby" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/mysql/mysql-original-wordmark.svg" title="MySQL"  alt="MySQL" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/nodejs/nodejs-original-wordmark.svg" title="NodeJS" alt="NodeJS" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/amazonwebservices/amazonwebservices-plain-wordmark.svg" title="AWS" alt="AWS" width="40" height="40"/>&nbsp;
<img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" title="Postman"  alt="Postman" width="40" height="40"/>&nbsp;
<img src="https://github.com/devicons/devicon/blob/master/icons/git/git-original-wordmark.svg" title="Git" **alt="Git" width="40" height="40"/>&nbsp;
</p>

---

### 🔥 &nbsp; My Stats :
[![GitHub Streak](http://github-readme-streak-stats.herokuapp.com?user=itsZed0&theme=dark&background=000000)](https://git.io/streak-stats)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=itsZed0&layout=compact&theme=vision-friendly-dark)](https://github.com/anuraghazra/github-readme-stats)

---













## Hi, I'm Fayas! 👋

- 📚 I'm currently studying computer science.
- 💻 I'm passionate about software development.
- 🌐 I'm interested in web design and development.
- 🔭 I enjoy working with the Python programming language.
- 🎯 I'm focused on improving my coding skills.
- 🌍 I love exploring new technologies and learning different programming languages.
- 🚀 I actively contribute to open-source projects and the developer community.
- 🎨 In my free time, I create open-source repositories.
- 📖 I constantly expand my knowledge through online courses and tutorials.
- 💡 I'm always seeking new challenges and opportunities to grow as a developer.
- 📫 You can reach me [via my accounts](https://fayasnoushad.github.io/#accounts).


===========================================
 IPython: Productive Interactive Computing
===========================================




 ![Language](https://img.shields.io/github/languages/top/thehassantahir/faceboom?style=for-the-badge)
 ![issues](https://img.shields.io/github/issues/thehassantahir/faceboom?style=for-the-badge)
 ![codesize](https://img.shields.io/github/languages/code-size/thehassantahir/faceboom?style=for-the-badge)
 ![license](https://img.shields.io/github/license/thehassantahir/faceboom?style=for-the-badge)
 ![forks](https://img.shields.io/github/forks/thehassantahir/faceboom?style=for-the-badge)
 ![stars](https://img.shields.io/github/stars/thehassantahir/faceboom?style=for-the-badge)
 ![twitter](https://img.shields.io/twitter/follow/thehassantahir?style=for-the-badge)


<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="hassan-tahir.github.io">
    <img src="https://github.com/thehassantahir/Faceboom/blob/master/img/faceboom-cover.png" alt="Logo">
  </a>

  <p align="center">
    A Social-Engineering Brute force application to hack facebook accounts!
    <br />
    <a href="https://github.com/hassan-tahir/Faceboom/wiki"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/hassan-tahir/Faceboom/issues">Report Bug</a>
    ·
    <a href="https://github.com/hassan-tahir/Faceboom/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#upcoming">Upcoming</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project



Faceboom is a brute force application built on python 2.7 later upgraded to 3.6 which enables the tester to enter the victims account by using their API, it uses various libraries like optparse, re and more.

How does it work?
* Faceboom is social engineering application, User can only hack the victims account if they are good in guessing and assuming other people trades and values.
* It uses wordlist to perform a sucessful hack, all the way the user have to update the wordlist.txt file which is already provided to make a hack attempt.


A list of commonly used resources that I find helpful are listed in the acknowledgements.

### Built With

* [Python](https://www.python.org/)


<!-- GETTING STARTED -->
## Getting Started

How to get this application run?

### Prerequisites

* For Linux installation 
  ```
  cd faceboom
  chmod +x setup.sh
  ./setup.sh
  ```
* For Windows installation
  * install python3 from python.org
  * install git from https://git-scm.com/downloads

### Usage

1. This program does not requie any installation because of run-time.
2. Clone the repo
   ```sh
   git clone https://github.com/thehassantahir/faceboom
   ```
3. Get into the directory of the program
   ```sh
   cd faceboom
   ```
4. Run your program
   ```sh
   python3 faceboom.py
   ```
5. Check the PATH and WAY
   ```sh
   python3 faceboom.py -h
   ```
   
  ### Upcoming
  
  1. Requirements.txt file {NEW FEATURE}
  2. .exe for Windows
  3. GUI for both env (Linux, Windows)

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.


<!-- CONTACT -->
## Contact

Twitter - [@thehassantahir](https://twitter.com/thehassantahir)

Website: [https://thehassantahir.web.app](https://thehassantahir.web.app)

[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png







<p align="center">
	<a href="https://thehassantahir.me" target="_blank"><img src="https://github.com/thehassantahir/thehassantahir/blob/main/github-banner.png"></a>
</p>

# react-simple-pull-to-refresh

[![npm version](https://badge.fury.io/js/react-simple-pull-to-refresh.svg)](https://badge.fury.io/js/react-simple-pull-to-refresh)
[![license](https://img.shields.io/github/license/thmsgbrt/react-simple-pull-to-refresh.svg)](https://github.com/thmsgbrt/react-simple-pull-to-refresh/blob/master/LICENSE)
![](https://badgen.net/npm/types/react-simple-pull-to-refresh)
![](https://badgen.net/badge/maintained/yes/green)

A Simple Pull-To-Refresh Component for React Application with 0 dependency.
Works for Mobile and Desktop.

## Contributing

⚠️ I don't have much time to take care of the issues at the moment.

🙏 Any help and contribution is greatly appreciated.

## Demo

[Click here 👍](https://thmsgbrt.github.io/react-simple-pull-to-refresh)

## Installation

`npm i react-simple-pull-to-refresh`

## Usage

```jsx
import PullToRefresh from 'react-simple-pull-to-refresh';
```

Pull To Refresh only

```jsx
// ...

return (
  <PullToRefresh onRefresh={handleRefresh}>
    <ul>
      {list.map((item, index) => (
        <li key={index}>{item}</li>
      ))}
    </ul>
  </PullToRefresh>
);

// ...
```





## Changelog

1.3.3: Update package.json peerDependencies to support react 18 - (From: [@mjauernig](https://github.com/mjauernig))

1.3.2: Fix build issue encountered with 1.3.1

1.3.1: Fix issue preventing fixed elements to work properly - (From: [@ManuDoni](https://github.com/ManuDoni))

1.3.0: Add a _resistance_ prop, that allows to adjust the pull down difficulty - (From: [@joshuahiggins](https://github.com/joshuahiggins))

1.2.5: Fix event listenter leaks - (From: [@d-s-x](https://github.com/d-s-x))

1.2.4: Fix overscroll on iOS Safari - (From: [@d-s-x](https://github.com/d-s-x))

1.2.3: Add React 17+ as valid peer dependencies - (From: [@Felixmosh](https://github.com/felixmosh))

1.2.2: Remove non-null assertion operators from ref.current + TouchEvent check for Mozilla - (From: [@HamAndRock](https://github.com/HamAndRock))

1.2.1: Remove unnecessary z-index

1.2.0: onRefresh and onFetchMore now require to be of type () => Promise<any>

1.1.2: Bind Scroll event to Window

1.1.0: Check for "canFetchMore" value for each scroll events.

1.1.0: Add a Fetch More feature















<h1><img src="https://emojis.slackmojis.com/emojis/images/1531849430/4246/blob-sunglasses.gif?1531849430" width="30"/> Hey! Nice to see you.</h1>


<p>Welcome to my page! </br> I'm Thomas, Fullstack developer from <img src="https://cdn-icons-png.flaticon.com/512/197/197560.png" width="13"/> <b>Lorient, France</b>, currently living in <img src="https://cdn-icons-png.flaticon.com/512/197/197564.png" width="13"/> <b>Stockholm, Sweden</b>. </p>
<h3>Things I code with</h3>
<p>
  <img alt="React" src="https://img.shields.io/badge/-React-45b8d8?style=flat-square&logo=react&logoColor=white" />
  <img alt="Webpack" src="https://img.shields.io/badge/-Webpack-8DD6F9?style=flat-square&logo=webpack&logoColor=white" /> 
  <img alt="Docker" src="https://img.shields.io/badge/-Docker-46a2f1?style=flat-square&logo=docker&logoColor=white" />
  <img alt="github actions" src="https://img.shields.io/badge/-Github_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white" />
  <img alt="Google Cloud Platform" src="https://img.shields.io/badge/-Google_Cloud_Platform-1a73e8?style=flat-square&logo=google-cloud&logoColor=white" />
  <img alt="TypeScript" src="https://img.shields.io/badge/-TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white" />
  <img alt="Insomnia" src="https://img.shields.io/badge/-Insomnia-5849BE?style=flat-square&logo=insomnia&logoColor=white" />
  <img alt="Apollo" src="https://img.shields.io/badge/-Apollo%20GraphQL-311C87?style=flat-square&logo=apollo-graphql&logoColor=white" />
  <img alt="Heroku" src="https://img.shields.io/badge/-Heroku-430098?style=flat-square&logo=heroku&logoColor=white" />
  <img alt="redux" src="https://img.shields.io/badge/-Redux-764ABC?style=flat-square&logo=redux&logoColor=white" />
  <img alt="ReactiveX" src="https://img.shields.io/badge/-RxJs-B7178C?style=flat-square&logo=reactivex&logoColor=white" />
  <img alt="GraphQL" src="https://img.shields.io/badge/-GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white" />
  <img alt="Sass" src="https://img.shields.io/badge/-Sass-CC6699?style=flat-square&logo=sass&logoColor=white" />
  <img alt="Styled Components" src="https://img.shields.io/badge/-Styled_Components-db7092?style=flat-square&logo=styled-components&logoColor=white" />
  <img alt="git" src="https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white" />
  <img alt="NestJs" src="https://img.shields.io/badge/-NestJs-ea2845?style=flat-square&logo=nestjs&logoColor=white" />
  <img alt="angular" src="https://img.shields.io/badge/-Angular-DD0031?style=flat-square&logo=angular&logoColor=white" />
  <img alt="npm" src="https://img.shields.io/badge/-NPM-CB3837?style=flat-square&logo=npm&logoColor=white" />
  <img alt="html5" src="https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" />
  <img alt="Brave browser" src="https://img.shields.io/badge/-Brave_Browser-FB542B?style=flat-square&logo=brave&logoColor=white" />
  <img alt="Rollup" src="https://img.shields.io/badge/-Rollup-EC4A3F?style=flat-square&logo=rollup.js&logoColor=white" />
  <img alt="d3js" src="https://img.shields.io/badge/-D3.js-F9A03C?style=flat-square&logo=d3.js&logoColor=white" />
  <img alt="Prettier" src="https://img.shields.io/badge/-Prettier-F7B93E?style=flat-square&logo=prettier&logoColor=white" />
  <img alt="MongoDB" src="https://img.shields.io/badge/-MongoDB-13aa52?style=flat-square&logo=mongodb&logoColor=white" />
  <img alt="Nodejs" src="https://img.shields.io/badge/-Nodejs-43853d?style=flat-square&logo=Node.js&logoColor=white" />
</p>
<h3>Open source projects</h3>
<table>
  <thead align="center">
    <tr border: none;>
      <td><b>🎁 Projects</b></td>
      <td><b>⭐ Stars</b></td>
      <td><b>📚 Forks</b></td>
      <td><b>🛎 Issues</b></td>
      <td><b>📬 Pull requests</b></td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://github.com/thmsgbrt/react-simple-pull-to-refresh"><b>React PullToRefresh component</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/thmsgbrt/react-simple-pull-to-refresh?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/thmsgbrt/react-simple-pull-to-refresh?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Issues" src="https://img.shields.io/github/issues/thmsgbrt/react-simple-pull-to-refresh?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/thmsgbrt/react-simple-pull-to-refresh?style=flat-square&labelColor=343b41"/></td>
    </tr>
	  <tr>
      <td><a href="https://github.com/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack"><b>Typescript & React Chrome Extension Starter</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Issues" src="https://img.shields.io/github/issues/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/thmsgbrt/Chrome-Extension-with-React-and-Typescript-Starter-Pack?style=flat-square&labelColor=343b41"/></td>
    </tr>
    <tr>
      <td><a href="https://github.com/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter"><b>NodeJs Express TypeScript GraphQL Starter</b></a></td>
      <td><img alt="Stars" src="https://img.shields.io/github/stars/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Forks" src="https://img.shields.io/github/forks/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Issues" src="https://img.shields.io/github/issues/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter?style=flat-square&labelColor=343b41"/></td>
      <td><img alt="Pull Requests" src="https://img.shields.io/github/issues-pr/thmsgbrt/nodejs-typescript-express-apollo-graphql-starter?style=flat-square&labelColor=343b41"/></td>
    </tr>
  </tbody>
</table>


<h3>Välkommen till <img src="https://cdn-icons-png.flaticon.com/512/197/197564.png" width="13"/> Stockholm!</h3>
<p><img width="200" src="" /> <img width="200" src="" /> <img width="200" src="" /></p>
<p>Above are the last 3 pictures posted by <a href="https://www.instagram.com/visitstockholm/" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e7/Instagram_logo_2016.svg/1024px-Instagram_logo_2016.svg.png" width="20"/> @visitstockholm!</a><br/>Currently, the weather is: <b> 3°C, <i>overcast clouds</i></b></br>Today, the sun rises at <b>08:43</b> and sets at <b>14:47</b>.</p>
<h3>Where to find me</h3>
<p><a href="https://github.com/thmsgbrt" target="_blank"><img alt="Github" src="https://img.shields.io/badge/GitHub-%2312100E.svg?&style=for-the-badge&logo=Github&logoColor=white" /></a> <a href="https://twitter.com/Guibz16" target="_blank"><img alt="Twitter" src="https://img.shields.io/badge/twitter-%231DA1F2.svg?&style=for-the-badge&logo=twitter&logoColor=white" /></a> <a href="https://www.linkedin.com/in/thomas-guibert" target="_blank"><img alt="LinkedIn" src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" /></a> <a href="https://medium.com/@th.guibert" target="_blank"><img alt="Medium" src="https://img.shields.io/badge/medium-%2312100E.svg?&style=for-the-badge&logo=medium&logoColor=white" /></a>
</p>

------------
<p align="center">This <i>README</i> file is generated <b>every 3 hours</b>!</br>Last refresh: Friday, 20 December, 01:03 CET<br /><a href="https://medium.com/@th.guibert/how-to-create-a-self-updating-readme-md-for-your-github-profile-f8b05744ca91">Create your own here!</a></p>
<p align="center"><img src="https://github.com/thmsgbrt/thmsgbrt/workflows/README%20build/badge.svg" /> <img alt="Stars" src="https://img.shields.io/github/stars/thmsgbrt/thmsgbrt?style=flat-square&labelColor=343b41"/> <img alt="Forks" src="https://img.shields.io/github/forks/thmsgbrt/thmsgbrt?style=flat-square&labelColor=343b41"/></p>













## Hi there 👋

<!--
**veffo/veffo** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->


Whoami 👤
Tools of Trade 🛠️
Experience 👨‍💼💼
Languages 📝🗣️
Volunteering 🙋‍♂️

## Table of contents
## Tools of Trade
- Web: Node.js, React.js, TailwindCSS
- Database: PostgreSQL, MySQL, MongoDB
- Containerization: Docker, Kubernetes, Rancher
- Cloud Computing: Digital Ocean, MVPS, Microsoft Azure, AWS
- CI/CD: TravisCI, CircleCI, Jenkins
- Scripting/Automation: Shell, CMD, Python, Ansible
- IAC: CloudFormation
- Server Administration: Linux, Windows, Nginx, Apache
- Computer Vision: Intel® OpenVINO Toolkit, OpenCV
- Artificial Intelligence: Microsoft Azure Studio

## Experience
My professional experience cuts across computer engineering, networking, systems administration and software development. See my Linkedin profile for more info.

## Languages
English (Professional)
Yoruba (Native)

<p align="center">
  <a href="https://getbootstrap.com/">
    <img src="https://getbootstrap.com/docs/5.3/assets/brand/bootstrap-logo-shadow.png" alt="Bootstrap logo" width="200" height="165">
  </a>
</p>

<h3 align="center">Bootstrap</h3>

<p align="center">
  Sleek, intuitive, and powerful front-end framework for faster and easier web development.
  <br>
  <a href="https://getbootstrap.com/docs/5.3/"><strong>Explore Bootstrap docs »</strong></a>
  <br>
  <br>
  <a href="https://github.com/twbs/bootstrap/issues/new?assignees=-&labels=bug&template=bug_report.yml">Report bug</a>
  ·
  <a href="https://github.com/twbs/bootstrap/issues/new?assignees=&labels=feature&template=feature_request.yml">Request feature</a>
  ·
  <a href="https://themes.getbootstrap.com/">Themes</a>
  ·
  <a href="https://blog.getbootstrap.com/">Blog</a>
</p>


## Bootstrap 5

Our default branch is for development of our Bootstrap 5 release. Head to the [`v4-dev` branch](https://github.com/twbs/bootstrap/tree/v4-dev) to view the readme, documentation, and source code for Bootstrap 4.


## Table of contents

- [Quick start](#quick-start)
- [Status](#status)
- [What's included](#whats-included)
- [Bugs and feature requests](#bugs-and-feature-requests)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [Community](#community)
- [Versioning](#versioning)
- [Creators](#creators)
- [Thanks](#thanks)
- [Copyright and license](#copyright-and-license)


## Quick start

Several quick start options are available:

- [Download the latest release](https://github.com/twbs/bootstrap/archive/v5.3.3.zip)
- Clone the repo: `git clone https://github.com/twbs/bootstrap.git`
- Install with [npm](https://www.npmjs.com/): `npm install bootstrap@v5.3.3`
- Install with [yarn](https://yarnpkg.com/): `yarn add bootstrap@v5.3.3`
- Install with [Composer](https://getcomposer.org/): `composer require twbs/bootstrap:5.3.3`
- Install with [NuGet](https://www.nuget.org/): CSS: `Install-Package bootstrap` Sass: `Install-Package bootstrap.sass`

Read the [Getting started page](https://getbootstrap.com/docs/5.3/getting-started/introduction/) for information on the framework contents, templates, examples, and more.


## Status

[![Build Status](https://img.shields.io/github/actions/workflow/status/twbs/bootstrap/js.yml?branch=main&label=JS%20Tests&logo=github)](https://github.com/twbs/bootstrap/actions/workflows/js.yml?query=workflow%3AJS+branch%3Amain)
[![npm version](https://img.shields.io/npm/v/bootstrap?logo=npm&logoColor=fff)](https://www.npmjs.com/package/bootstrap)
[![Gem version](https://img.shields.io/gem/v/bootstrap?logo=rubygems&logoColor=fff)](https://rubygems.org/gems/bootstrap)
[![Meteor Atmosphere](https://img.shields.io/badge/meteor-twbs%3Abootstrap-blue?logo=meteor&logoColor=fff)](https://atmospherejs.com/twbs/bootstrap)
[![Packagist Prerelease](https://img.shields.io/packagist/vpre/twbs/bootstrap?logo=packagist&logoColor=fff)](https://packagist.org/packages/twbs/bootstrap)
[![NuGet](https://img.shields.io/nuget/vpre/bootstrap?logo=nuget&logoColor=fff)](https://www.nuget.org/packages/bootstrap/absoluteLatest)
[![Coverage Status](https://img.shields.io/coveralls/github/twbs/bootstrap/main?logo=coveralls&logoColor=fff)](https://coveralls.io/github/twbs/bootstrap?branch=main)
[![CSS gzip size](https://img.badgesize.io/twbs/bootstrap/main/dist/css/bootstrap.min.css?compression=gzip&label=CSS%20gzip%20size)](https://github.com/twbs/bootstrap/blob/main/dist/css/bootstrap.min.css)
[![CSS Brotli size](https://img.badgesize.io/twbs/bootstrap/main/dist/css/bootstrap.min.css?compression=brotli&label=CSS%20Brotli%20size)](https://github.com/twbs/bootstrap/blob/main/dist/css/bootstrap.min.css)
[![JS gzip size](https://img.badgesize.io/twbs/bootstrap/main/dist/js/bootstrap.min.js?compression=gzip&label=JS%20gzip%20size)](https://github.com/twbs/bootstrap/blob/main/dist/js/bootstrap.min.js)
[![JS Brotli size](https://img.badgesize.io/twbs/bootstrap/main/dist/js/bootstrap.min.js?compression=brotli&label=JS%20Brotli%20size)](https://github.com/twbs/bootstrap/blob/main/dist/js/bootstrap.min.js)
[![Backers on Open Collective](https://img.shields.io/opencollective/backers/bootstrap?logo=opencollective&logoColor=fff)](#backers)
[![Sponsors on Open Collective](https://img.shields.io/opencollective/sponsors/bootstrap?logo=opencollective&logoColor=fff)](#sponsors)


## What's included

Within the download you'll find the following directories and files, logically grouping common assets and providing both compiled and minified variations.

<details>
  <summary>Download contents</summary>

  ```text
  bootstrap/
  ├── css/
  │   ├── bootstrap-grid.css
  │   ├── bootstrap-grid.css.map
  │   ├── bootstrap-grid.min.css
  │   ├── bootstrap-grid.min.css.map
  │   ├── bootstrap-grid.rtl.css
  │   ├── bootstrap-grid.rtl.css.map
  │   ├── bootstrap-grid.rtl.min.css
  │   ├── bootstrap-grid.rtl.min.css.map
  │   ├── bootstrap-reboot.css
  │   ├── bootstrap-reboot.css.map
  │   ├── bootstrap-reboot.min.css
  │   ├── bootstrap-reboot.min.css.map
  │   ├── bootstrap-reboot.rtl.css
  │   ├── bootstrap-reboot.rtl.css.map
  │   ├── bootstrap-reboot.rtl.min.css
  │   ├── bootstrap-reboot.rtl.min.css.map
  │   ├── bootstrap-utilities.css
  │   ├── bootstrap-utilities.css.map
  │   ├── bootstrap-utilities.min.css
  │   ├── bootstrap-utilities.min.css.map
  │   ├── bootstrap-utilities.rtl.css
  │   ├── bootstrap-utilities.rtl.css.map
  │   ├── bootstrap-utilities.rtl.min.css
  │   ├── bootstrap-utilities.rtl.min.css.map
  │   ├── bootstrap.css
  │   ├── bootstrap.css.map
  │   ├── bootstrap.min.css
  │   ├── bootstrap.min.css.map
  │   ├── bootstrap.rtl.css
  │   ├── bootstrap.rtl.css.map
  │   ├── bootstrap.rtl.min.css
  │   └── bootstrap.rtl.min.css.map
  └── js/
      ├── bootstrap.bundle.js
      ├── bootstrap.bundle.js.map
      ├── bootstrap.bundle.min.js
      ├── bootstrap.bundle.min.js.map
      ├── bootstrap.esm.js
      ├── bootstrap.esm.js.map
      ├── bootstrap.esm.min.js
      ├── bootstrap.esm.min.js.map
      ├── bootstrap.js
      ├── bootstrap.js.map
      ├── bootstrap.min.js
      └── bootstrap.min.js.map
  ```
</details>

We provide compiled CSS and JS (`bootstrap.*`), as well as compiled and minified CSS and JS (`bootstrap.min.*`). [Source maps](https://web.dev/articles/source-maps) (`bootstrap.*.map`) are available for use with certain browsers' developer tools. Bundled JS files (`bootstrap.bundle.js` and minified `bootstrap.bundle.min.js`) include [Popper](https://popper.js.org/docs/v2/).


## Bugs and feature requests

Have a bug or a feature request? Please first read the [issue guidelines](https://github.com/twbs/bootstrap/blob/main/.github/CONTRIBUTING.md#using-the-issue-tracker) and search for existing and closed issues. If your problem or idea is not addressed yet, [please open a new issue](https://github.com/twbs/bootstrap/issues/new/choose).


## Documentation

Bootstrap's documentation, included in this repo in the root directory, is built with [Hugo](https://gohugo.io/) and publicly hosted on GitHub Pages at <https://getbootstrap.com/>. The docs may also be run locally.

Documentation search is powered by [Algolia's DocSearch](https://docsearch.algolia.com/).

### Running documentation locally

1. Run `npm install` to install the Node.js dependencies, including Hugo (the site builder).
2. Run `npm run test` (or a specific npm script) to rebuild distributed CSS and JavaScript files, as well as our docs assets.
3. From the root `/bootstrap` directory, run `npm run docs-serve` in the command line.
4. Open `http://localhost:9001/` in your browser, and voilà.

Learn more about using Hugo by reading its [documentation](https://gohugo.io/documentation/).

### Documentation for previous releases

You can find all our previous releases docs on <https://getbootstrap.com/docs/versions/>.

[Previous releases](https://github.com/twbs/bootstrap/releases) and their documentation are also available for download.


## Contributing

Please read through our [contributing guidelines](https://github.com/twbs/bootstrap/blob/main/.github/CONTRIBUTING.md). Included are directions for opening issues, coding standards, and notes on development.

Moreover, if your pull request contains JavaScript patches or features, you must include [relevant unit tests](https://github.com/twbs/bootstrap/tree/main/js/tests). All HTML and CSS should conform to the [Code Guide](https://github.com/mdo/code-guide), maintained by [Mark Otto](https://github.com/mdo).

Editor preferences are available in the [editor config](https://github.com/twbs/bootstrap/blob/main/.editorconfig) for easy use in common text editors. Read more and download plugins at <https://editorconfig.org/>.




## Versioning

For transparency into our release cycle and in striving to maintain backward compatibility, Bootstrap is maintained under [the Semantic Versioning guidelines](https://semver.org/). Sometimes we screw up, but we adhere to those rules whenever possible.

See [the Releases section of our GitHub project](https://github.com/twbs/bootstrap/releases) for changelogs for each release version of Bootstrap. Release announcement posts on [the official Bootstrap blog](https://blog.getbootstrap.com/) contain summaries of the most noteworthy changes made in each release.











## Copyright and license

Code and documentation copyright 2011–2024 the [Bootstrap Authors](https://github.com/twbs/bootstrap/graphs/contributors). Code released under the [MIT License](https://github.com/twbs/bootstrap/blob/main/LICENSE). Docs released under [Creative Commons](https://creativecommons.org/licenses/by/3.0/).








































# A collection of `.gitignore` templates

This is GitHub’s collection of [`.gitignore`][man] file templates.
We use this list to populate the `.gitignore` template choosers available
in the GitHub.com interface when creating new repositories and files.

For more information about how `.gitignore` files work, and how to use them,
the following resources are a great place to start:

- The [Ignoring Files chapter][chapter] of the [Pro Git][progit] book.
- The [Ignoring Files article][help] on the GitHub Help site.
- The [gitignore(5)][man] manual page.

[man]: http://git-scm.com/docs/gitignore
[help]: https://help.github.com/articles/ignoring-files
[chapter]: https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#_ignoring
[progit]: http://git-scm.com/book

## Folder structure

We support a collection of templates, organized in this way:

- The root folder contains templates in common use, to help people get started
  with popular programming languages and technologies. These define a meaningful
  set of rules to help get started, and ensure you are not committing
  unimportant files into your repository.
- [`Global`](./Global) contains templates for various editors, tools and
  operating systems that can be used in different situations. It is recommended
  that you either [add these to your global template](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files#configuring-ignored-files-for-all-repositories-on-your-computer)
  or merge these rules into your project-specific templates if you want to use
  them permanently.
- [`community`](./community) contains specialized templates for other popular
  languages, tools and project, which don't currently belong in the mainstream
  templates. These should be added to your project-specific templates when you
  decide to adopt the framework or tool.

## What makes a good template?

A template should contain a set of rules to help Git repositories work with a
specific programming language, framework, tool or environment.

If it's not possible to curate a small set of useful rules for this situation,
then the template is not a good fit for this collection.

If a template is mostly a list of files installed by a particular version of
some software (e.g. a PHP framework), it could live under the `community`
directory. See [versioned templates](#versioned-templates) for more details.

If you have a small set of rules, or want to support a technology that is not
widely in use, and still believe this will be helpful to others, please read the
section about [specialized templates](#specialized-templates) for more details.

Include details when opening pull request if the template is important and visible. We
may not accept it immediately, but we can promote it to the root at a later date
based on interest.

Please also understand that we can’t list every tool that ever existed.
Our aim is to curate a collection of the _most common and helpful_ templates,
not to make sure we cover every project possible. If we choose not to
include your language, tool, or project, it’s not because it’s not awesome.

## Contributing guidelines

We’d love for you to help us improve this project. To help us keep this collection
high quality, we request that contributions adhere to the following guidelines.

- **Provide a link to the application or project’s homepage**. Unless it’s
  extremely popular, there’s a chance the maintainers don’t know about or use
  the language, framework, editor, app, or project your change applies to.

- **Provide links to documentation** supporting the change you’re making.
  Current, canonical documentation mentioning the files being ignored is best.
  If documentation isn’t available to support your change, do the best you can
  to explain what the files being ignored are for.

- **Explain why you’re making a change**. Even if it seems self-evident, please
  take a sentence or two to tell us why your change or addition should happen.
  It’s especially helpful to articulate why this change applies to _everyone_
  who works with the applicable technology, rather than just you or your team.

- **Please consider the scope of your change**. If your change is specific to a
  certain language or framework, then make sure the change is made to the
  template for that language or framework, rather than to the template for an
  editor, tool, or operating system.

- **Please only modify _one template_ per pull request**. This helps keep pull
  requests and feedback focused on a specific project or technology.

In general, the more you can do to help us understand the change you’re making,
the more likely we’ll be to accept your contribution quickly.

## Versioned templates

Some templates can change greatly between versions, and if you wish to contribute
to this repository we need to follow this specific flow:

- the template at the root should be the current supported version
- the template at the root should not have a version in the filename (i.e.
  "evergreen")
- previous versions of templates should live under `community/`
- previous versions of the template should embed the version in the filename,
  for readability

This helps ensure users get the latest version (because they'll use whatever is
at the root) but helps maintainers support older versions still in the wild.

## Specialized templates

If you have a template that you would like to contribute, but it isn't quite
mainstream, please consider adding this to the `community` directory under a
folder that best suits where it belongs.

The rules in your specialized template should be specific to the framework or
tool, and any additional templates should be mentioned in a comment in the
header of the template.

For example, this template might live at `community/DotNet/InforCRM.gitignore`:

```
# gitignore template for InforCRM (formerly SalesLogix)
# website: https://www.infor.com/product-summary/cx/infor-crm/
#
# Recommended: VisualStudio.gitignore

# Ignore model files that are auto-generated
ModelIndex.xml
ExportedFiles.xml

# Ignore deployment files
[Mm]odel/[Dd]eployment

# Force include portal SupportFiles
!Model/Portal/*/SupportFiles/[Bb]in/
!Model/Portal/PortalTemplates/*/SupportFiles/[Bb]in
```

## Contributing workflow

Here’s how we suggest you go about proposing a change to this project:

1. [Fork this project][fork] to your account.
2. [Create a branch][branch] for the change you intend to make.
3. Make your changes to your fork.
4. [Send a pull request][pr] from your fork’s branch to our `main` branch.

Using the web-based interface to make changes is fine too, and will help you
by automatically forking the project and prompting to send a pull request too.

[fork]: https://help.github.com/articles/fork-a-repo/
[branch]: https://help.github.com/articles/creating-and-deleting-branches-within-your-repository
[pr]: https://help.github.com/articles/using-pull-requests/

## License

[CC0-1.0](./LICENSE).




















# Hi [<img src="https://github.com/dlirA01/dlirA01/blob/main/wave.gif" width="28px"/>][youtube], I'm Arild or as i'm known on here, [Alien][youtube] [<img src="https://github.com/dlirA01/dlirA01/blob/main/wink-tounge.gif" width="28px"/>][youtube]

<br />

## Graphic designer, programmer & photographer

- 🌼 Currently studying digital media and design

<br />

## Connect with me

[<img src="https://github.com/dlirA01/dlirA01/blob/main/youtube.svg" height="12px"/>][youtube] [YouTube][youtube] &nbsp;&nbsp;
[<img src="https://github.com/dlirA01/dlirA01/blob/main/twitter.svg" height="12px"/>][twitter] [Twitter][twitter] &nbsp;&nbsp;
[<img src="https://github.com/dlirA01/dlirA01/blob/main/instagram.svg" height="12px"/>][instagram] [Instagram][instagram] &nbsp;&nbsp;
[<img src="https://github.com/dlirA01/dlirA01/blob/main/codepen.svg" height="12px"/>][codepen] [Codepen][codepen]

<br />
<br />

---

<details>
<summary>:star: Github Stats</summary>

  <br />
  
  <!-- start -->
  [![dlirA01's github stats](https://github-readme-stats.vercel.app/api?username=dlirA01&count_private=true&show_icons=true&theme=omni)](https://github.com/dlirA01/github-readme-stats)
  <!-- end -->

</details>

[youtube]: https://youtube.com/ArealAlien
[twitter]: https://twitter.com/Areal_Alien
[instagram]: https://instagram.com/areal_alien
[codepen]: https://codepen.io/areal_alien







<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 2000 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**
- **[WebReinvent](https://webreinvent.com/?utm_source=laravel&utm_medium=github&utm_campaign=patreon-sponsors)**
- **[Lendio](https://lendio.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
















<!--
repo name: Md-Template
description: An awesome readme Template extension to quickstart your project
github name:  oGranny
link: https://github.com/oGranny/readme-template-extension
logo path: assets/logo.png
screenshot: 
twitter: your_username
email: example@email.com
-->

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->



<!-- PROJECT LOGO -->
<br />
<p align="center">
    <a href="https://github.com/oGranny/readme-template-extension">
        <img src="icon.png" alt="Logo" width="80" height="80">
    </a>
<h3 align="center"><a href="https://github.com/oGranny/readme-template-extension">readme-template-extension</a></h3>
    <p align="center">
        An awesome readme Template extension to quickstart your project
        <br />
        <a href="https://marketplace.visualstudio.com/items?itemName=oGranny.md-template"><strong>Visual studio market place 📃</strong></a>
        <br />
        <br />
        <a href="//github.com/Md-Template/ oGranny">View Demo</a>
        •
        <a href="https://github.com/oGranny/readme-template-extension/issues">Report Bug</a>
        •
        <a href="https://github.com/oGranny/readme-template-extension/issues">Request Feature</a>
    </p>
</p>



<!-- TABLE OF CONTENTS -->
## Table of Contents

- [Table of Contents](#table-of-contents)
- [About The Project](#about-the-project)
  - [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)



<!-- ABOUT THE PROJECT -->
## About The Project

There are many great README templates available on GitHub, however, I didn't find one that really suit my needs so I created this enhanced one. I want to create a README template so amazing that it'll be the last one you ever need.

Here's why:
* Your time should be focused on creating something amazing. A project that solves a problem and helps others
* You shouldn't be doing the same tasks over and over like creating a README from scratch
* You should element DRY principles to the rest of your life 😄:

Of course, no one template will serve all projects since your needs may be different. So I'll be adding more in the near future. You may also suggest changes by forking this repo and creating a pull request or opening an issue.

A list of commonly used resources that I find helpful are listed in the acknowledgements.

### Built With
* [yo]()
* [vsce]()


<!-- GETTING STARTED -->
## Getting Started
* Download the extension
* write `!!!` and click on the first option (make sure you are editing a markdown file)

### Prerequisites

* [VS Code](https://code.visualstudio.com)

### Installation

download this extension directly from VS code [marketplace](https://marketplace.visualstudio.com/vscode)



<!-- USAGE EXAMPLES -->
## Usage

vscode extension for github readme snippet to quick start your project



<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/oGranny/readme-template-extension/issues) for a list of proposed features (and known issues).



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

oGranny - ogranny.github.io@gmail.com

Project Link: [https://github.com/oGranny/readme-template-extension](https://github.com/oGranny/readme-template-extension)



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/oGranny/readme-template-extension.svg?style=flat-square
[contributors-url]: https://github.com/oGranny/readme-template-extension/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/oGranny/readme-template-extension.svg?style=flat-square
[forks-url]: https://github.com/oGranny/readme-template-extension/network/members
[stars-shield]: https://img.shields.io/github/stars/oGranny/readme-template-extension.svg?style=flat-square
[stars-url]: https://github.com/oGranny/readme-template-extension/stargazers
[issues-shield]: https://img.shields.io/github/issues/oGranny/readme-template-extension.svg?style=flat-square
[issues-url]: https://github.com/oGranny/readme-template-extension/issues
[license-shield]: https://img.shields.io/github/license/oGranny/readme-template-extension.svg?style=flat-square
[license-url]: https://github.com/oGranny/readme-template-extension/blob/master/LICENSE.txt
[product-screenshot]: images/screenshot.png



















<!--
**Ileriayo/ileriayo** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
--->  

<h1 align="center"> 👋 </h1>
<div align="center">
  <img src="https://github.com/Ileriayo/ileriayo/blob/master/images/header.gif" alt="header"/>
</div>
<p align="center"> (Open for Hiring)</p>

<h2 align="center"> 👨‍💻 Whoami</h2>
<p align="center">
  <samp>A highly resourceful computer programmer and well-rounded IT professional with over five years of computing experience, possessing expert knowledge of the software development lifecycle and a solid understanding of technologies required for the development and deployment of highly available and scalable applications, including their networks and infrastructure.
  </samp>
  <br> <br>
  <img src="https://komarev.com/ghpvc/?username=ileriayo" alt="https://github.com/ileriayo" />
</p>

<hr>

<h2 align="center"> 🔭 Tools of Trade</h2>
<p align="center">
  <img src="https://img.shields.io/badge/node.js%20-%2343853D.svg?&style=for-the-badge&logo=node.js&logoColor=white" />&nbsp;&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/react%20-%2300D9FF.svg?&style=for-the-badge&logo=react&logoColor=white" />&nbsp;&nbsp;&nbsp;
  <img src="https://img.shields.io/badge/tailwind-css%20-%231572B6.svg?&style=for-the-badge&logo=tailwind-css&logoColor=white" />&nbsp;&nbsp;
</p>
<p align="center">TailwindCSS, Python, Docker, Kubernetes, Rancher, TravisCI, Git, Github, Bitbucket, Apache, Nginx, Vagrant, Ansible, Jenkins, Azure.</p>

<hr>

<h2 align="center">💬 My Blog Articles</h2>
<p align="center" align='right'>
  <a target="_blank"href="https://dev.to/ileriayo"><img src="https://img.shields.io/badge/dev.to-%2312100E.svg?&style=for-the-badge&logo=dev.to&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;
  <a target="_blank"href="https://medium.com/@ileriayoadebiyi"><img src="https://img.shields.io/badge/Medium%20-%231572B6.svg?&style=for-the-badge&logo=medium&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;
</p>

<hr>

<h2  align="center">📫 Reach me on</h2>
<p align="center">
  <a target="_blank"href="https://www.linkedin.com/in/ileriayo-adebiyi-0328b1101/"><img src="https://img.shields.io/badge/linkedin-%230077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
  <a target="_blank"href="https://twitter.com/ileriayooo"><img src="https://img.shields.io/badge/twitter-%231DA1F2.svg?&style=for-the-badge&logo=twitter&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="mailto:ileriayoadebiyi@gmail.com?subject=Hello%20Ileri,%20From%20Github"><img src="https://img.shields.io/badge/gmail-%23D14836.svg?&style=for-the-badge&logo=gmail&logoColor=white" /></a>&nbsp;&nbsp;&nbsp;&nbsp;
</p>

<hr>

<h2  align="center">💻 Check Out My Repos ⬇️ </h2>

















<p align="center"><a href="https://anuraghazra.github.io"><img width="80%" alt="Hello, I'm Anurag. I do open source!" src="./assets/gh-readme-header.png" /></a></p>

<br />

I'm a self-taught passionate FrontEnd developer from India 🇮🇳

**About me**

- 💼 FrontEnd Engineer at [Razorpay](http://razorpay.com/)

- 📈 Built github-readme-stats, verlyjs and more, **50m+** hits • **50K** stars on GitHub

- ❤️ I love writing TypeScript, and building fun experiments on type-level

- 💬 Ask me about anything [here](https://github.com/anuraghazra/anuraghazra/issues)

<code><img height="20" alt="javascript" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/javascript/javascript.png"></code>
<code><img height="20" alt="typescript" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/typescript/typescript.png"></code>
<code><img height="20" alt="react" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/react/react.png"></code>
<code><img height="20" alt="graphql" src="https://raw.githubusercontent.com/github/explore/5c058a388828bb5fde0bcafd4bc867b5bb3f26f3/topics/graphql/graphql.png"></code>
<code><img height="20" alt="nodejs" src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/nodejs/nodejs.png"></code>    


| <a href="https://github.com/anuraghazra/github-readme-stats"><img align="center" src="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&include_all_commits=true&theme=buefy&hide_border=true" alt="Anurag's github stats" /></a> | <a href="https://github.com/anuraghazra/github-readme-stats"><img align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=anuraghazra&layout=compact&theme=buefy&hide_border=true" /></a> |
| ------------- | ------------- |

#### Top Repositories


<a href="https://github.com/anuraghazra/github-readme-stats">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=github-readme-stats&theme=buefy" />
</a>
<a href="https://github.com/anuraghazra/anuraghazra.github.io">
  <img align="center" src="https://github-readme-stats.vercel.app/api/pin/?username=anuraghazra&repo=anuraghazra.github.io&theme=buefy" />
</a>

<br />
<br />

<a href="https://twitter.com/anuraghazru">
  <img align="right" alt="Anurag Hazra | Twitter" width="21px" src="https://raw.githubusercontent.com/anuraghazra/anuraghazra/master/assets/twitter.svg" />
</a>
<a href="https://codesandbox.io/u/anuraghazra">
  <img align="right" alt="Anurag Hazra | CodeSandbox" width="20px" src="https://raw.githubusercontent.com/anuraghazra/anuraghazra/master/assets/codesandbox.svg" />
</a>
