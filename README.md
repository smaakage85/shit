# Shit Commit

<p align="center">
<img src="logo.png" alt="Shit Commit" width="300"/>
</p>

`shit commit` is a convenient Git life-hack and productivity booster targeting lazy programmers. It works with both Linux and MacOS operating systems.

Without any further ado: **LET THE SHITSHOW BEGIN**! 

## Motivation

I often commit stuff to git. This implies me spending a shitload of keystrokes on (*): (1) staging all changes, (2) committing the changes and (3) pushing them to a remote branch: 

```bash
git add . 
git commit -m "[ARBITRARY COMMIT MESSAGE]"
git push
```

over and over and over again... 😴

### DO YOU RELATE?

How nice would it be, if you could somehow spare these shitty keystrokes and spend them on something less redundant, more productive...

.. And **YES**! It turns out, **you actually can**.

## **`shit commit`** to the rescue

Let me introduce you to your savior: **`shit commit`**. 

With `shit commit` you will never have to type all of that shit again. Let `shit commit` deal with it.

`shit commit` is a convenient bash function, that does (*) in one go: 

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
   # push to remote branch
   git push
}
```

## How to Start the Shit-storm

Append the above code snippet to your `.bashrc` file.

Restart the terminal:

```bash
$SHELL
```

That's it. You are now all set to make your first `shit commit`.

Next time you want to do (*), simply run:

```bash
shit
```

For every dump you take, this will save you for **more than 31 keystrokes** .

If you want to go the extra mile and provide your `shit commit` with a custom commit message, you can do it by:

```bash
shit "[COMMIT MESSAGE]"
```

## Frequently Asked Questions

**Q**: Should you not consider carefully what changes to commit in stead of just committing all changes? With this approach you risk pushing unintentional changes?

**A**: Well.. Shit happens! And since you are tracking your project with Git, you can always roll any unintended changes back.

**Q**: Should you not write a telling commit message, every time you commit your changes?

**A**: Nobody reads those messages anyway. Anyways, if you insist, you can provide your own custom message: `shit "[message]"`. 
