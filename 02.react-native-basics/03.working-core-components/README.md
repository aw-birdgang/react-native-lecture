
## install
```bash
    
```


## script
```bash

```


## description
```bash
So let's start by diving deeper

into core components like Text and View.

And for this I'll actually delete this status bar component

and also this import.

If I save that, this is updated here on those devices

and not much change here, so we don't need this right now.

I also will delete this Text component and save that,

so that for now we have a blank screen.

And now let's try re adding the text like this,

"Hello World" between the View,

without the surrounding text.

If we do that, we notice that we get an error down here.

We get an error that

"Text strengths must be rendered within a Text component"

which is actually a quite helpful error message

which tells us in a pretty clear way, what's wrong.

And before we fix this,

let's also take a look at those devices,

those simulators,

and here we also get the same error message.

And this is actually something important

which is why I'm showing this.

It's different than what you might know

from web development.

If you would build a web app,

and this would be react for the web

and this would maybe be a div instead of a View,

then this kind of code would be fine.

We could put text inside of a div there.

React Native and native platforms to be precise

are stricter than that.

You can't put a Text into a View

which is pretty much the equivalent to a div

because it's not meant for that.

Instead Views, so the of to divs in the web world,

Views are meant to generally build boxes

and containers that hold other content.

A View could hold some text wrapped into a Text component.

It could also hold a TextInput or a button

or an image, or anything like this,

but you have to put the content

into an element that is able to display it.

And the View is only able to hold other components,

It's not able to display text,

and that is something really important to understand.

If you wanna display a text, for example,

you have to use this Text component

and wrap the text opening and closing text around your text.

And if you do this and save, then this updates

and works again, but that's a first important takeaway

even though we can kind of compare those component to HTML.

And even though it looks kind of similar,

there are important differences.

Now, what you will often do when building React Native apps

is you will build more complex user interfaces

that don't just have one piece of text inside of them.

And what's important to understand then

is that those different core components

have different roles.

The Text is a component that's used for, guess what?

Displaying text.

The View is a component that's meant to hold

and lay out other components.

Now, we will learn more about laying things out

with help of styling in a couple of minutes,

but the idea behind the View component is that

you typically have multiple child components in there.

For example, another text,

"Another piece of text".

In a Text component, as you learned,

but now we got two of them.

And we grouped them together in a View

just as we might group them together in a div

if this would be for the web.

Now, in the web, we also have other components like section

or article, here in React Native world,

it's just the View.

This is our container component

that we use for holding our components.

And of course, those other components also can be nested.

We could have another View

which actually holds this inner text.

So this is all something that's totally fine,

something you will typically build when building

more complex user interfaces with React Native.

The View then makes it very easy to use styling

into which we'll dive in a second to control

where which of its child elements should be positioned.

Of course, we don't just have a View and Text to though.

If you take a look at the official website,

the official React Native documentation site

you'll learn that there are more

React Native core components

and those components fulfill different purposes.

We got View and Text, which are two of the most important

and commonly used components,

but we also could display a image, add some scrolling,

something will do later as well,

or add a TextInput which allows users to enter some text.

We could also add a button,

and indeed, that is what I'll do here.

Below this text, I'll add a button,

but for this, we need to import it.

And that is also important

and an important difference compared to react for the web.

With react for the web, you don't need to import

the HTL elements you might be using,

with React Native, you do.

If you wanna display a button,

you have to import this core component from React Native,

and then you can add your button.

And number important difference is that unlike for the web,

you don't build a button like this

by adding the caption between the opening and closing tags.

Instead, it's a self-closing element

where you add a title prop,

and then you add your title here.

This would now display a button as well

with the kind of default styling

and tap effects you would expect

for the different platforms.

And you see that the look adjusts

to the underlying platform.

It looks like an iOS button on iOS,

and like an Android button on Android.

But of course the button doesn't do anything yet

because I have added any listener.

Now, we will add interactivity,

and learn how that works later.

For the moment, let's just add the button here

and let's understand that we always work

with core components like this

where every component has its clearly defined purpose,

and you build your overall UI by combining those components.

But of course a UI is not just about combining components,

it's also about styling them,

and that's therefore what will explore next.
```
