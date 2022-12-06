
## install
```bash
    
```


## script
```bash

```


## description
```bash
So let's explore how we can build

real layouts where we don't just have a bunch of

centered texts and buttons.

And for this, I will actually clean up my JSX content

and I will remove this style prop here

on the outer view for the moment

and remove all the styling here in this style sheet object

but I will keep the style sheet object.

And now here in my view,

I actually wanna add a neverview

and below that a neverview.

Now I'm doing this because

I wanna start building a basic interface here

that allows us to manage goals.

And the first view,

the first nested view here I should say,

should actually hold the input area

where users can enter the text for their goal

and click a button to add that goal.

And the second view should later hold the list of goals

that are rendered.

And I'm using two views as rappers

to have a clear separation between these two areas,

and because data will help me with styling.

So for this, I'll then therefore start

by adding a text input component here in the first view.

This is a component that allows users to enter text

and like all components, all core components,

we need to import it from react-native.

Now text input is a self-closing component.

And here we can, for example, add some placeholder text

as you could add it to a input element in the web

and say, your course goal.

Then, next to it I want to add a button

with the title of add goal.

And then here in this view, I will add a text element

where I say, list of goals

and later this will become a real list.

Now, if we save all of that,

we see that everything is crunched here at the top.

We also see that it goes beneath the status bar

and there would be different ways of fixing this.

For the moment, I'll fix it

by giving this outer view a style prop

and defining a style, which I'll name, app container.

And in there I'll add a padding of, let's say, 50 pixels.

And then here we can refer to styles.appContainer

to add to this padding to the overall outer view.

Now, if you save this,

we can see that there's more space around our UI.

Again, later, we will learn about different ways

of making sure that we don't interfere

with those native status bars and so on.

Now, still, this is not the layout I want.

For example, I want the button to be next to this input,

not beneath it.

I also want to have more space between the list of goals

and maybe this area where we add a goal

should take up a quarter of the overall height

and the list should take up the rest.

And that's where we need new styling features.

Styling properties about which we haven't learned before.

Specifically, we need flex box.
```
