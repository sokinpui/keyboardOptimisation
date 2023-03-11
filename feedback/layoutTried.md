# Reason I change the layout.
I write code and type shell command often, I find my personal typing is not very 
efficient, so I make some change to alter the situation. There are change that I 
have tried:
1. chagne qwerty to any alternative
2. use layer to input symbols and number

I used to be believe that less key is better, so I try to implement a 40% 
keyboard layout on my macbook keyboard. Spacebar on Macbook is long, and it is 
uncomfortable to press left right command with thumbs, it makes it is difficult 
to implement thumbs layer switcher like planck's keyboard. Moreover, I find 
backspace is difficult to reach, I map caps `lock + space` as backspace and 
`quote` as `return` and a symbols layers, while I held down the `space` I can 
switch to the symbols layers. I use goku simlayers to implement the layers,
where I find it sometimes inconvenient since I need to press the right key 
immedently after held down `space`, if i don't then many `space` is inserted.  
If I use layers can solve this problem, however, when I type faster, the `space` 
itself is being eaten.

## Before design symbol layers
I try workman, dvoark, minimak, norman, colemak and colemak mod-dh. While they 
all claims that they are more efficient and comfortable than qwerty. Maybe they 
are true, but not ture for me. The most preferred non-qwerty layout is colemak 
mod-dh, but finally give up. I realise that I prefer my finger "dancing" on 
three rows instead of staying on home row. The feeling after trying few qwertyj

## First version
Held down `space` to enter symbol mode, all symbols is begin put into one layer 
make symbols live in a crowded space. And it is one of the reason it fail 
finally.
symbol layer at this time:
![first symbol layer](img/fistSymoblLayer.png?raw=true)

## why I give up this layer?
It don't work as expected, I used to think that not only cool and real efficient 
for typing and programming or type command in shell. The real is that it will
need more time to correct the mistake as error is easier to generate when using 
simlayers. 

## Second verison
In the second turn, I use dead key to implement the layers. Press `caps lock` to 
active symbols layers, press `enter` to active the number layer. Symbol layers 
will be inactive after the symbols is inserted. Number layers stay until I press 
the "escape" keys.
![second symbol layer](/img/secondSymbolLayer.png?raw=true)
![number layer](/img/numberLayer.png?raw=true)

## Give up again
Number layer is bad, It is inefficient and no necessary to press three key when 
you can simply type one "far away" number. Symbols layer is fine, after I 
realise that number row worth it, I start thinking what's wrong with the symbols 
on numbers? The main problem is that they need to work with shift. Number row is 
not far away, just move the finger forward a bit enough to reach the nubmer 
rows. I uncover that balance should be make between minimalism and efficient.  
When you can type one key that is actually not far, how can it be efficient to 
break down the key into combination? Still worse, I will need to combine number 
with command and symbols in vim. To avoid type too much unnecessary keys comb, I 
better adopt the true that less is not better when complexity increses.

# Conulsion
Qwerty is not bad.
single but "far" key >> keys combination

