# `shit commit`

`shit commit` is a convenient Git life-hack and productivity booster targeting lazy programmers. It works with both Linux and MacOS operating systems.

Without any further ado: let the shitshow begin! 

## Motivation

I often commit stuff to git. This implies me spending a shitload of keystrokes on (*): (1) staging all changes, (2) committing the changes and (3) pushing them to a remote branch: 

```bash
git add . 
git commit -m "[ARBITRARY COMMIT MESSAGE]"
git push
```

over and over and over again... 😴

Do you relate?

How nice would it be, if you could somehow spare these shitty keystrokes and spend them on something less redundant, more productive...

.. And **YES**! It turns out, **you actually can**.

## **`shit commit`** to the rescue

Let me introduce to your savior: **`shit commit`**. 

With `shit commit` you will never have to type all of that shit again yourself. Let `shit commit` deal with it.

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

## How to start the shit-storm

Append the above function to your `.bashrc` file.

Restart the terminal:

```bash
$SHELL
```

That's it. You are now all set to make your first `shit commit`.

Next time you want to do (*), simply run:

```bash
shit
```

in stead. For every dump you take, this will save you for more than **31 keystrokes** .

## FAQ



