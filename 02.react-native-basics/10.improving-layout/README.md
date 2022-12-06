
## install
```bash
    
```


## script
```bash

```


## description
```bash
So now after this deep dive, let's use

our newly gained knowledge to improve this overall layout.

One thing I will do for example,

is work on this app container padding.

This actually doesn't use any of the new knowledge

but I need to do this to make this look a bit prettier.

I basically just want to have a padding to the top of 50

and then I wanna have a padding horizontal,

so left and right of 16.

So not of 50 but of 16.

With that I'd say, this generally looks better,

though we can see that this padding is kind of ignored

and our button here is going off the screen.

This can be fixed by decreasing the amount of width

our text input has to 70% maybe.

Now this looks better.

What doesn't look better though is where this text is

in this button.

This is something we can improve with align items

on the input container though.

At the moment, the problem is that basically this button

is stretched to be as high as this text input.

And the text is then not centered in the button

because the button doesn't have any styles

that would center the text.

Now you could think that maybe we can add some styling

to the button but it turned out that the button

is a component that doesn't have a style prop.

It might look like it has because I'm getting

some auto completion here but that's actually only some

auto completion I get here because I typed the word style

before in this code file.

The proper auto completion that tells me that a certain prop

is supported looks like this with this kind of icon

next to it.

So the button doesn't have a style prop

because indeed it doesn't support styling.

You can always check out the official docs and dive into

an element there to see which props it supports.

And for example, on the button, there is no style prop.

Whereas on the view, for example, you do find a style prop.

But that's just a side note, that's why we have to fix it

differently and we can fix it by not stretching this button.

That would be one way of achieving this.

So we can set a line items here on input container

and set this to center instead of stretch.

With that, the button is now centered and looks better.

We could also build our own button

but that is something you will learn later.

So now this looks better.

I also wanna change how much space this input area takes up

though and how much space the list of goals takes up.

To achieve this, I'll do a couple of things.

For example, I wanna add some padding to the bottom

on this input container of let's say 24.

so that there is some space between the view that holds

the text input and the button and the view that will hold

the list of goals later.

You can see that spacing here now.

We also could add a little border here,

so we could add a border to the bottom

and give it a width by setting border bottom width of one.

And then adding a border to the bottom and giving it a color

of let's say, maybe this gray again.

But of course you can pick any color you want.

Now we got this border and below that to the list of goals.

But now I want to make sure that my text input area

takes up one fourth, so 1/4 of the overall available height.

And this can be done with the flex property

as you learned.

We can set this to one and then add a styling object

to this view that holds the list of goals

that takes up three quarters of the available space,

which can be achieved by adding flex three to this view.

So therefore I'll add another styling object

in my style sheet here and name it, the goals container.

And here I'll set flex three.

As you learned, all the flex values are added together

as long as the containers to which they are added

are siblings to each other and are part

of the same surrounding parent element which is the case

for these two views

and then the space is distributed accordingly.

So one plus three is four and therefore this takes

one fourth and this will take three quarters.

We just have to add this here, so I will add a style prop

to this view and set this equal to styles goals container.

With that, it will look horrible.

And the reason for this is that we also need to work

on the outer container now.

The container that holds these two containers

on which we just set the flex properties.

This outer container needs to take up the entire height

of the app so that the inner containers

can then distribute this space.

By default, without the flex property,

this container will only take as much space as it needs

and that's only defined by the space

the content in the container takes up.

But now that we're setting flex on those containers

in the container, this doesn't work anymore.

And to fix this, we need to force this container to take

all the available height and we do this by simply adding

flex one to the app container so that the outer container

takes all the height because it's the only container here.

So flex one will give it all the space

and then the inner containers can divide

that available space.

So by adding flex one to the app container and saving this,

this now looks better.

And now this is a quarter and that here are three quarters.

Now if I look at it like this,

this still doesn't look perfect so what we might wanna do

is actually give that list here 4/5 of the available space,

so that goals container will get four

and the input container stays at one.

And instead of setting a padding bottom,

I will set a margin bottom here on the input container.

And with that, that looks better.

We could maybe even go to flex five down there

and leave it like this.

Feel free to experiment with this

and choose your own values.

But this will work for me and this is now flex box in action

to achieve a first basic layout.

Of course, this is not the final layout we will have though.
```
