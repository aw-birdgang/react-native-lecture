
## install
```bash
    
```


## script
```bash

```


## description
```bash
So, let's dive into React Native.

For this, I'm back in this project

we created in the first course section.

In case you did not create it there

or you did remove it thereafter,

just make sure you got

the development environment set up mentioned there,

and then you can download

the attached starting project.

Once you did that, you will get the same code

as I have it here.

Just make sure that you open your terminal

or command prompt.

Here, I'm using the one integrated in this code

and that you install all the dependencies

this project needs, by running npm install.

And once that completed, you can run npm start

to this Expo process

that watches the code and builds the preview

and serves it on our emulators.

I'll then press a and i

to start and run this app

on my running Android and iPhone

emulators and simulators.

Here you go.

These are my two preview devices.

Now, and actually as we already got some code

on which we worked in the first course section already,

and what we have in here in the end

is a React component, a Functional React component.

And indeed, in this course,

we will only work with functional components

and React hooks.

We will not use class based components.

So this is a regular functional component.

We also got this Styles constant,

this SyleSheet object down there.

And I will come back to that in a couple of minutes.

At the top of this file, we got some imports

and we're importing one component

from an Expo related package.

And the other components, namely View and Text

as well as this SyleSheet object here,

from React Native.

And Text and View are two

of those built in components,

actually two of the most important

built in components,

React Native exposes to you,

to use in your JSX code.

Because in here, you can't use divs or h2 tags

or anything like this.

These are HTML elements, which work in the browser

when you have a DOM to work with,

but they won't work here on a Native device,

because Native devices are not browsers.

They don't have that DOM,

and they don't support those HTML elements.

Keep this slide from the first course section in mind,

that is how React Native translates different elements

into different Native elements

for Android and iOS.

And that's why these components are exposed

by React Native.

Now, if you visit the official React Native website,

then there, you will find various guides

which you can definitely take a look at

but you will also find the components tab

where you get a list of the components

provided by React Native.

And as you can tell,

we actually don't have that many components here

because it turns out

that with a couple of core components,

you can build any kind of user interface.

For example, we got a Button here

and Image and Text and View.

And especially View and Text and Text Input

are super important components

which you will use all the time.

And as you will learn from this course,

you can build very complex user interfaces

with those core components that you have here.

Now, React Native is all about working

with those core components that are built into it.

You build your overall app UI

and your custom components

that might make up that UI,

by simply combining those core components.

Because these core components, as you learned,

are translated into Native UI widgets,

Native UI elements for Android and iOS

by a React Native.

That's why we work with those core components

that are provided by React Native.

And we can combine them in our React Code,

in our JSX code, to build our own components

and ultimately our own user interface.

So in the end, we just compose our components

by combining those core opponents.

And if you think about it,

that's the same for React for the web.

HTML happens to have more elements.

There are h1, h2 elements, divs, article section,

there are many HTML elements.

But in the end, you also just combine

those HTML elements to build the web user interface.

It's the same here for Native apps.

So that's what we do with those components.

Of course, another important aspect

of building user interfaces in general

is that you wanna style those apps.

And when using React Native, there is no CSS.

You can't write CSS code,

because again, it's not a browser,

so the CSS language doesn't exist here.

Instead, you can, of course, still apply Styles,

but you do this either in line,

essentially by using props

on those core components that are provided

or with help of these SyleSheet objects

or this SyleSheet object

which you already saw in the code before.

You therefore. write your styling in JavaScript.

And hence, you have no extra styling language.

It's all JavaScript, but the React Native team

gives you a lot of JavaScript properties

which you can set and pass to those core elements,

which are similar to the CSS properties.

But it's only a subset

of the overall CSS property and feature set.

But in the end, as you will learn

throughout this Course,

you get all the important CSS properties

and features that you need

to build powerful and beautiful user interfaces.

But back here in our component code,

we can see how these core components

that are provided by React Native

are combined to build a new component,

in this case, the only component, the app component,

and how we then get this StyleSheet object,

which is used to set various styles

which if you take a look at those properties,

look similar to what you know from CSS.

And then actually this Styles object is provided

to this View component through a style prop.

But we will take a closer look at styling

and at building our own components in general

throughout the next minutes and hours, of course.

Now, just one final note about this app component:

At the moment, this is our only component here.

And indeed the app component in the app JS file

has a special purpose.

This is the root component

that is rendered in your app.

Expo will automatically take this component,

export it in this app JS file,

and render this as the root component.

So, any other user interface elements and components

must go into this app component

or into children or descendants of this app component.

But again, that is also something we'll explore

in greater details soon.
```
