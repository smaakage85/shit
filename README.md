<p align="center">
<img src="logo.png" alt="Shit Commit" width="300"/>
</p>

`shit commit` is a next-level Git life-hack and productivity booster targeting lazy programmers. It works with both Linux and MacOS operating systems.

I promise you, Git will never be the same again.

Without any further ado: **LET THE SHITSHOW BEGIN**! 

## Motivation

I often commit stuff to Git. This implies me spending a shitload of keystrokes on (*): 

1. Staging all changes
2. Committing the changes
3. Pushing them to a remote branch

all the time. The same **36+** keystrokes:

```bash
> git add . 
> git commit -m "[ARBITRARY COMMIT MESSAGE]"
> git push
```

over and over and over again... 😴

**.. CAN YOU RELATE?**

Imagine how nice it would be if you could somehow spare these shitty keystrokes and spend them on something less redundant, more productive...

.. And **YES**! It turns out, **you actually can**.

## `shit commit` to the Rescue

Let me introduce you to your savior: `shit commit`. 

With `shit commit` you will never have to type any of that shit again. Let `shit commit` deal with it.

`shit commit` consists of a convenient bash function, that does (*) in one go: 

```bash
# shit commit
function shit() {
   msg="$USER rocks this shit!"
   if [ ! -z "$1" ]; then
     msg="$1"
   fi
   # stage all changes
   git add .
   # commit changes
   git commit -m "$msg"
   # push changes to remote branch
   git push
}
```

## Start the Shit-storm

Shit is about to get real!

Append the above code snippet to your `.bashrc` file.

Restart the terminal:

```bash
> $SHELL
```

That's it. You are now all set to make your first `shit commit`.

Next time you want to do (*), simply run:

```bash
> shit
```

As you see, it only takes **5** keystrokes. FIVE! Consequently, for every dump you take, `shit commit` will save you for **more than 31 keystrokes**.

If you want to go the extra mile and provide your `shit commit` with a custom commit message, you can do it by:

```bash
> shit "[COMMIT MESSAGE]"
```

<p align="center">
<img src="shit.gif" alt="Walkthrough"/>
</p>

## Frequently Asked Questions

**Q**: Should you not consider carefully what changes to commit instead of just committing all changes? With this approach you risk pushing unintended changes?

**A**: Well.. Shit happens! And since you are tracking your project with Git, you can always roll any unintended changes back.

**Q**: Should you not write a telling commit message, every time you commit your changes?

**A**: Nobody reads those messages anyway. But if you insist, you can provide your own custom message like this: `shit "[message]"`. 

## 'Shit' Count
22

## Cite this work

```
@inproceedings{shitcommit,
  title = {Shit Commit},
  author = {Kjeldgaard, Lars},
  year = {2022},
  publisher = {GitHub},
  url = {https://github.com/smaakage85/shit}
}
```