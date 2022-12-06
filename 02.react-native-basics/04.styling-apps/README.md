
## install
```bash
    
```


## script
```bash

```


## description
```bash
So let's dive into styling.

And here you learned before

that there is no CSS support in the React Native,

so we don't add CSS files

or use the CSS language in general,

but you learned that we have two main ways of adding styling

by either adding styles in line,

by passing a style object to props

or by defining a separate object

which is then also passed through props.

Now we do define our styles in JavaScript then

but the JavaScript properties we can set

are inspired by the CSS language

though it's only a subset of the properties

and features supported by CSS

and not all the names are exactly the same, as you will see.

But let's now see how styles can be applied.

For that, we can use the style prop,

which is not supported on all elements,

but on some elements, for example on the view,

but also on the text.

For example, here on let's say this text here,

we can add the style prop.

And then as a value, you can pass a JavaScript object.

And in this object you can set

all the supported style properties and React Native decides

which properties are supported.

And these are the properties that are similar

to the CSS properties, but not exactly the same.

For example, here on this text, we could add a margin.

And as you see, as I start typing,

we get this nice auto completion here in VS Code.

We get this automatically because VS Code understands

which kind of properties can be set on this object

that is passed to the style prop.

Now, here we could add a margin

either in one specific direction or in multiple directions

by combining multiple properties

or in all directions by setting margin.

Now different style properties

need different kinds of values.

And you will see many examples

and learn which kind of value goes into which style property

throughout this course.

Margin, for example, typically wants a number

and this number will then be translated to pixels

which are automatically adjusted

to the device pixel density.

For example, here we could enter 16

to have a margin of 16 pixels.

If we save this, we got some spacing around this.

Now it's not super good to see

because we don't know exactly where the text box ends.

To make this a bit more visible, we could add a border.

Now in Vanilla CSS, you could add a border,

like this for example.

This would add a red border with one pixel width

around an element in Vanilla CSS.

But if I type this kind of code

and saved this here in React Native,

we actually got no effect here,

and I got a error here in the terminal

and a warning here on my simulator.

We can click on this to get more details

and we see that this is an invalid value for border.

Actually the key border already is invalid.

So it's not even the value

but border is not a supported key.

The reason for this is simply

that this border property doesn't exist.

I mentioned that the styling language is inspired by CSS

and close to CSS, but it's not exactly the same.

Instead, as we type border,

we see that various properties exist, which we can set.

For example, we can set a border with property

and this again wants a number to set

a certain border width in pixels, like one, one pixel,

or two or whatever you want.

And then we can also set a bordered color.

Now this does not want a number, but instead of string,

and in this string, you could define a hex code value

Or you provide one of the supported shortcuts

like red or blue or green or black and white.

And here I will go for red.

And this will now add a two pixel, white, red border

around this text.

Now I'll press the auto format shortcut

to make this a bit easier to read and then save this.

And with this, we now got a border around this text.

The border is pretty close to the text

but thankfully we can also add some padding,

padding just as in the browser,

is the spacing inside of an element.

So here we could add a padding of let's say 16 again,

16 pixels, just as for the margin.

And if we save this and auto format again

to improve readability, now we got some internal spacing.

Now definitely feel free to play around more

with those style properties.

And of course also take a look at the official docs

to learn more about styling if you want to,

but you will see plenty of styling examples

throughout the course.

These style properties were all about styling

the element itself that holds a certain piece of content.

We will later also learn about style properties

that help us with laying out multiple components

and with achieving a certain overall look.

But again, that is something we will explore later.

For the moment,

I wanna leave this in-line styling approach though.

This approach of defining the styles in the same line

as we define this component.

Because whilst this is possible and allowed,

it's rarely the best way of adding styling.

So typically we should go for a style sheet objects.

The reason for this,

is that this allows us to clearly separate

our JSX code and our styling code

and it also makes our styles reusable.

If we define styles in line

and I want the same styling on this text,

I have to copy and paste this,

so that I can add my style prop here

and add the same styling,

and I'll auto format this to make it more readable.

So now I had to copy and paste to replicate this style.

And that is typically something you wanna avoid.

What you should instead do

is create a new style sheet object.

Or if you already have one, as we have it here,

you go to this object and you add a new property.

We already have the container property,

now on the same level, I'm adding another property.

The name is up to you and I'll just name it dummy text.

Again, this is totally up to you.

What's not up to you is what you set as a value though.

The value should be an object,

as we see it here for a container.

And then in this object, you define your style properties.

So here I could now set my margin and so on.

So I can set margin 16, border width two and border color,

I'll set this to red.

And I will all set my padding and the order does not matter.

I just group margin and padding together here,

since they're both about spacing,

but we could also add padding here,

and it wouldn't matter.

Of course I could have also just copied down

my object from up here.

Now with such a style object to find down here,

we can use it here in our JSX code

as this container is being used.

It is defined down here, but you can still use it

in JSX because this only gets executed

after the entire code file has been parsed basically.

So here we can now replace this object

by referring to styles.dummytext

and I get nice auto completion for this as well.

And I'll do this here as well.

And now, yes, we had to copy the word, dummy text,

but of course it's way less to copy.

And if we ever adjust the style,

for example we changed the color to blue,

we don't have to do this in two places

because the name didn't change,

we just had to do it in one place instead.

So if I save this, we now got a blue border.

And that's how we use such a style sheet object.

Now, why is it a style sheet object?

So an object created with help of style sheet create

which is a built-in method on this built-in object

which is imported from React Native.

Well, we could have also created

a styles object like this, and set our styles there,

but using such a style sheet object has the advantage

that we get convenient auto completion

as we type our style properties here.

And that makes our development life a bit easier.

In addition, React Native could potentially optimize

style sheet creation and management internally

and pick up style sheet objects like this.

This is not done right now though,

so for the moment, the main reason is the auto completion.

But with that, we now learn some important styling basics

and some important basics about core components.

I would say, as a next step,

we should take a closer look at creating layouts

and positioning multiple elements

because typically you don't just want

a couple of centered pieces of text like this.

Typically you are going for different layouts

and we need to know how we can create

such layouts therefore.
```
