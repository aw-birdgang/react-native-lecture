
## install
```bash
    
```


## script
```bash
http://reactnative.dev/docs/flexbox

```


## description
```bash
In this lecture,

I wanna dive a bit deeper into Flexbox especially regarding

how you use it in React Native apps.

If you know all about that already,

you can of course skip this lecture.

So for this, I prepared a simple dummy application

and of course, you find data attached.

It's a normal React Native app built with Expo.

And in the App.js file here,

what I have in the end, is just a view with three views

in there where each view then has a text

with text one, two, three.

This simply creates some boxes

with different colors, red, blue, and green.

And now we'll use Flexbox to move these boxes around

so that you can get a feeling for how Flexbox works,

because it's so important.

Now, first things first, by default,

every view in React Native,

even if you assign no special styles, uses Flexbox.

And that's different to the web, for example.

There, if you have a div, which would be your equivalent

to a view kind of,

it doesn't use Flexbox by default.

In React Native, it does.

Every view by default organizes its children

with the help of this Flexbox thing.

Flexbox simply is, is a term,

It's simply a concept from CSS

that is all about organizing child elements

in a one dimensional space.

So here, for example, in a column.

That's also in every default,

not only does every view by default you use Flexbox,

it also by default organizes children in a column,

so from top to bottom.

That's all the difference to the web

and I don't wanna emphasize these differences too much

because of course you don't need to be a web developer

to build React Native apps.

But I think a lot of people do know web development,

do know a CSS Flexbox, and therefore it makes sense

to all the talk about the differences.

So in the web, when you use Flexbox

not only is it not turned on by default,

in addition if you do turn it on,

the default is to organize all child elements in a row.

And here, the default is to organize them in a column.

You can change that default though.

So in this case, on the view, which holds my boxes

by adding flexDirection here,

and setting this to row, for example.

Now, you will see that these three boxes are organized

in a row from left to right.

Now besides row and column,

you also have row reverse and column reverse.

And this simply also, well does what the name implies,

now we still have a row,

but the first element, the red box, actually is on the right

and not on the left anymore.

So that's also something you can do.

Let me go back to row view.

So that's the first thing you can do.

Another important thing about Flexbox

is how child elements are sized.

Here, I gave every child element

a width and a height of 100.

Now, if we would remove that width and height thing

on every child element, then you will see

that now we have a very, very small row here

because every box now is only as wide

as its child requires it to be.

And only as tall as its child requires it to be.

So every box here which holds a number

is only as wide and tall as the number it's containing.

Now, you can change that

with the surrounding Flexbox container 2.

Let's give that width of let's say 300 pixels

or of 80% of the parent width.

So in this case,

since it's the root element of the device width,

and let's give it a height of, let's say 300.

If we do that, and now really important,

I'm doing this on the view, which holds all these boxes.

I'm not doing it on the boxes themselves.

So if we assign this width and height

on the surrounding box, you see something interesting.

The height is assumed for all the elements.

Now, all the views

in the Flexbox take the height of the parent.

The width has no impact here.

That's also a default behavior you got here,

obviously since we haven't changed anything.

The default behavior here indeed, is that the child elements

in a Flexbox, so in this outer view here,

are organized such that they align themselves

along the cross axis by stretching.

Okay, that were a lot of terms,

what does this mean?

Now, when working with Flexbox,

we have two important axis.

The main axis depends on your flex direction.

For row, which we have here, flex direction row.

the main axis is from left to right.

For a row reverse, it would be right to left.

For column, it would be top to bottom

and for column reverse it would be bottom to top.

So that's the main axis.

And then you also have a cross axis

and that's simply the opposite of the main axis.

So for a row where the main axis is from left to right

the cross axis would be from top to bottom.

If the main axis is from right to left

which would be the case for row reverse

then the cross axis would be from bottom to top.

Okay, so that's the main axis and cross axis concept.

Now, you can organize your child elements.

So in this view where we have the free boxes

as child elements,

you can organize these child elements along these axis.

You use justifyContent to organize elements

along the main axis.

And you have alignItems to organize elements

around the cross axis.

Now you see the values you got for justifyContent here.

If you add these quotes

or if you place your cursor in there

and you hit control+space.

You see you can center elements, you can position them

at the end or at the start of that container

or you can add some space in between.

For example, if we use space between here

and we use alignItems center, then things will change.

Now, you will see they're taking the width

of the surrounding container,

every box itself still is pretty small

but they're split or they're distributed

across the width of the parent container.

And they're no longer taking the height

because along the cross axis,

we're aligning them with align items.

And there I set this to center.

The default here is stretch.

And if I set it back to stretch,

then unsurprisingly they do stretch for the entire height.

Now, if you want to make sure

that they take the available width,

you can set stretch here on justify content

which is your main axis positioning vehicle.

So you can set stretch here.

So what can you do regarding that then?

Well, that is something you now configure

on every child item itself.

You can tell a child item how much space it should take

off the space it's potentially getting.

Stretch here is kind of a special case,

there you set this up on the parent item.

Normally, you set this up on the child item.

So for example, if I set this to center now

so that the parent doesn't tell the child

how much space it should take.

then we can fully control the space a child takes

by going to the child style.

And there you can add flex, the flex property.

The flex property is applied

to items that are inside of a Flexbox,

so that are inside of a view in this case here.

And that can be a view itself

but that could also be another component

like a text, for example.

So now here you can add flex

and you can set this to a value of one, for example.

So flex needs to be a number.

If you set this to one,

what you will see is that now the red container

where I did set flex to one,

takes all the available width it can get

just so much that it leaves enough space

for the blue and the green container

so that they can squeeze their content

into the surrounding Flexbox.

Now, we can't see the boundaries

of the surrounding container

but the boundaries would essentially be where

the red item starts

and the green item ends on the horizontal axis here.

So now flex 1 makes sure

that the red item gets as big as it can get,

So it takes as much space as it can get.

but default views only take as much space

as their child elements require.

So as this one character required,

but with flex one you change this

and they now take as much space along the main axis.

So along the width here, as they can get.

For the cross axis, again, that's a special case,

You have to do this on the parent.

For the main axis, and since we have row here,

the main axis is a horizontal axis from left to right,

you do this with the flex property on a child.

Now, of course you can add flex

to other child elements as well.

Like to the second, to the blue container,

with the two in there.

You can add flex 1 there as well.

So now I have flex 1 on the red container

and flex 1 on the blue container.

And what now happens is that both of them

take the available free space, and amongst these two boxes,

the space is distributed evenly.

And that's what this number here indicates.

This number is a relative number.

All items in the same Flexbox

with the flex property distribute the available space

by considering the number you assign here.

And these numbers are relative to each other,

so if I give the blue container flex 2 here,

then this means that of the available space you have

in that surrounding container.

After deducting the space,

every element needs to squeeze its content in there.

The blue container will take twice as much space

as this one, because here we have flex 1,

here we have flex 2.

If we had flex 3 here,

then this would take three fifths

of the available free space,

because we have three plus two,

so we have five available segments, so to say.

And here the red container would take three segments,

blue container would take two segments.

If we have one and two,

then we have three available segments,

and the blue container takes two of them,

red takes one.

So you always add up these flex numbers

and then distribute or that's automatically done, of course

but then the available space is distributed accordingly.

So now here we'll see

that the blue container is twice as big as the red one

or it takes twice as much free space as the red one.

So this is how you can work with flex.

You can organize how items are positioned

with flex-direction, with justify content

and with align items.

And you can also make your items grow

and shrink the help of flex.

So now that's our brief introduction to Flexbox

in React Native.

As I said, inspired by Flexbox for CSS.

So if you knew that,

all of what I explained here is probably not new to you.

We'll work with Flexbox throughout this course,

so there're things also will become clearer

and we'll work a lot with it.

And you'll see you how you can create beautiful

user interfaces with Flexbox.

Flexbox in the end is the tool

in React Native to structure your content

on a page, to organize your content.

And you would typically work with a lot of views

which you also nest into each other

so that you can position elements the way you want.

Because of course, and that's also important,

you don't just have to have one view in your app

which uses Flexbox.

You could have another view

in there which also uses Flexbox.

And actually, as I mentioned

every view by default uses Flexbox

and you can then nest these views into each other

so that you position everything the way you want.

And you'll also see this in this module already.

And actually I'm already doing it here in my views here

which are in the surrounding view.

So my boxes here, there I also use justifyContent

and alignItems to center my numbers in these boxes.

So that one, two and three are centered there

horizontally and vertically.

And that works because we have Flexbox turned

on by default and we can't turn it off by the way.

And therefore, I just use these two properties here

to align my content of this view

along the main and the cross axis.

And here, since I have set no special flex direction

for this view, the main axis is top to bottom

because the default flex direction is column

and the cross axis is left to right.

That's just a side note.
```
