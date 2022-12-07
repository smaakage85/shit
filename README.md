# shit commit

A convenient life-hack and productivity booster targeting lazy programmers.

Works with OS: Linux/MacOS.

## Motivation

I often commit stuff to git, so I spend a shitload of key strokes on typing (*):

```bash
git add . 
git commit -m "[ARBITRARY COMMIT MESSAGE]"
git push
```

over and over and over again... 😴

Do you relate?

How nice would it be, if you could somehow spare these shitty key strokes and spend them on something less redundant, more productive...

.. And **YES**! It turns out, **you actually can**.

## 'shit commit' to the rescue

Let me introduce to your savior: '**shit commit**'. 

With 'shit commit' you will never have to type all of that shit again yourself. 'shit commit' will deal with it.

'shit commit' is a convenient bash function. 

```bash
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

## FAQ



