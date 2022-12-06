# :shit: SHIT COMMIT

A life-hack for lazy programmers.

## Deep shit

I often commit stuff to git. I have spent a shitload key strokes on typing:

```bash
git add .
git commit -m "[SOME ARBITRARY COMMIT MESSAGE UNDERSTANDABLE FOR ABSOLUTELY NOONE ELSE]"
git push
```

How nice would it be, if I could somehow spare these key strokes...

**WELL, YOU ACTUALLY CAN!**

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

