# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Takže než začneme, jak *ty* čteš?

`publish("show_options_bottom")`

# intro-start-2

n3: Pojďme začít náš příběh...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: TOTO JE ČLOVĚK

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: A TOTO JE JEHO ÚZKOST

n: _TY_ JSI ÚZKOST

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Nope. No, nope, not listening. Gonna check my phone.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: MUSÍŠ ČLOVĚKA CHRÁNIT PŘED *NEBEZPEČÍM*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Hej! Zase už zahazuješ čas sjížděním Twitteru!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Divím se proč si vlastně nesednu a neposlouchám myšlenky častěji.

`hong({eyes:"neutral"});`

n: RYCHLE, VARUJ JI PŘED *NEBEZPEČÍM*!

```
bb({eyes:"look"});
```

[Ale ne, podívej se na tuhle příšernou novinku!](#act1d_news)

[Ale ne, není tenhle tweet tajně o *nás*?](#act1d_subtweet)

[Hele, GIF kde kočka pije mléko!](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Jéé, to je roztomílé, já--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KOČKY NEZVLÁDNOU ZTRÁVIT MLÉKO A MY JSME HROZLÍ LIDÉ, PROTOŽE SI UŽÍVÁME MUČENÍ ZVÍŘAT

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



