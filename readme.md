#  Notes

## Animation Syntax
The @keyframe syntax for animation goes like this:
```
@keyframes name {
    sequence {
        parameters
    }
}
```

So for something like `rotation`, we can have something like:
```
@keyframes spin {
    to {
        transform: rotate(360deg);
    }
}
```
In the element we want to rotate, say a div with id #rotate, we write:

```
#rotate {
    animation-duration: 2s;
    animation-name: spin;
}
```

And we have a basic spin animation. 

## Keep animation running
As observed, these animations only ran once. This is where `animation-iteration-count` comes in. To keep the animation running in perpetuity, you can add the word `infinite` or specify an actiual number. 

```
animation-iteration-count: 5;
```