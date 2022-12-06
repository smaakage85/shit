# :shit: Shit Commit

A git life-hack for lazy programmers.

## Motivation

I often commit stuff to git. I have spent a shitload of key strokes on typing:

```bash
git add .
git commit -m "[SOME ARBITRARY COMMIT MESSAGE UNDERSTANDABLE FOR ABSOLUTELY NOONE ELSE THAN ME]"
git push
```

How nice would it be, if I could actually somehow spare these key strokes...

.. And **YES! you actually can**.

## The solution

Let me introduce to you: **SHIT COMMIT**.

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



