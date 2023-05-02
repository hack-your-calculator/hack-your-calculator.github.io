---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Game - Guessing Game
---

![thinking](/images/thinking.webp){:height="280px" .centered-image}

```basic
ClrHome

randInt(1,100)→N

Disp "Guess a number"
For(T,1,10)
 Input "Guess?",G
 If N=G:Then
  Disp "You've got it!","Guesses:",T
  Pause 
  Return
 Else
  If N>G:Then
   Disp "Higher…"
  Else
   Disp "Lower…"
  End
 End
End

Disp "You lose!","The number was:",N
```