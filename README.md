# :shit: shit commit

A git life-hack for lazy programmers.

## Motivation

I often commit stuff to git, so I spend a shitload of key strokes on typing:

```bash
git add .
git commit -m "[SOME ARBITRARY COMMIT MESSAGE UNDERSTANDABLE FOR ABSOLUTELY NOONE ELSE THAN ME]"
git push
```

again and again and again and...

Do you relate?

How nice would it be, if you could actually somehow spare these key strokes and spend them on something less redundant, more productive...

.. And **YES! It turns out, you actually can**.

## Introducing 'shit commit'

Let me introduce to you: '**shit commit**'.

```bash
function shit() {
   msg="$USER rocks this shit!"
   if [ ! -z "$1" ]; then
     msg="$1"
   fi
   git add .
   git commit -m "$msg!"
   git push
}
```

## FAQ



