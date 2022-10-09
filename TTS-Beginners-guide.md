# Getting Started Guide

Credit to **SensorLock** from the Command Point Discord for running [me](https://github.com/veddermatic) through this. Note that this guide was written by someone completely new to TTS (**Lumpy** on Command Point Discord), so it may contain extra steps, or there might be easier ways to accomplish things. This is how I was able to reproduce what I was shown so others can benefit.

By the end of this guide, you will have a kill team roster with all the models you need, and all the models on your roster will be set up with **KT Command Node** which makes playing a lot more streamlined. You will also get walked through using **KT UI Extender** which is something you'll use during games to make things even easier and faster while you play.

## Assumptions

This guide assumes the following:

- You have TableTop Simulator (TTS) installed.
- A web browser.
- You have the ability to create a BattleScribe Roster file.
- You have subscribed to the following Workshop items:
  - [All Kill Teams in Boxes](https://steamcommunity.com/sharedfiles/filedetails/?id=2699529917)
  - [KT Command Node](https://steamcommunity.com/sharedfiles/filedetails/?id=2614731381)
  - [KT Map Base](https://steamcommunity.com/sharedfiles/filedetails/?id=2574389665)
  - [KT UI Extender](https://steamcommunity.com/sharedfiles/filedetails/?id=2722788048)

Doing these things is outside the scope of this document for now. Feel free to add help for these things!

## Pre-Game

There are a bunch of things you can do before you play to get set up and save time; namely loading models and your roster, then getting them associated with a **KT Command Node**

## Get your team's models

This step will get your factions models saved as a custom object so you can quickly load them wherever you want them.

1. Fire up TTS
2. Click `Create -> Single Player`
3. Select `Workshop -> All Kill Teams In Boxes`
4. After a moment, you will see boxes with every kill team!
5. Find your faction / team and click the `place` button next to the box.
6. The models will load and appear on the table (this may take a moment)
7. Left-click & drag to select all the models
8. Right-click and pick `save object`
9. Change the name to something smart like "MyFaction's Models"

You can now load your models into any game you play easily.

## Setting up KT Command Node

**KT Command Node** is an add-on that gives your models extra functionality, like adding / removing wounds and other Kill Team related things. This makes life in-game so much easier, but it requires using BattleScribe and a web app. You'll upload your roster to Data Team, which will store it, and punch the code it gives you into KT Command Node so it can load your roster and do the facny things it does with it.

### Outside of TTS

1. Create a Kill Team ROSTER (not a Kill Team) in BattleScribe (or some other thing that can make BattleScribe roster files.)
2. Add all the units you think you _might_ use in a game to your roster (over do it)
3. Ensure there are no errors on your roster (everyone has guns / options selected)
4. You _can_ add equipment at this point, but as of this writing, it is probably best to leave it off for now.
5. Once your roster is error free and full, save it as a BattleScribe roster file.
6. Go to the [Data Team web app](https://datateam.app/Encode) and load your roster file
7. After a moment, it will say `Your Roster Code is:`
8. Copy and paste that Roster Code in a text file or write it down in case it magically leaves your clipboard.

### Back in TTS

1. Go back to the main Menu if you already have a game going
2. Pick `Create -> Single Player`
3. Load `KT Map Base Table`
4. Pick `Games -> Workshop`
5. Find `KT Command Node` and click on the three dots in the top right.
6. Pick `Additive Load`
7. A Hexagonal token will appear.
8. Hover over it, right click and pick `save object`
9. Save it as "blank kz command node" or something clever like that.
10. Delete the Command Node you just placed. (do we need this step and the next one?)
11. Add a copy of command node you just saved via `Objects -> Saved Objects` and clicking on your command node. Click on the table to place it.
12. Load in your faction's models that you saved in the first step in via `Objects -> Saved Objects` and clicking on your models. Click on the table to place them. Put them near the command node for ease. I suggest up and to the left or right of it relative to the label on the token.

### Now it is time for the magic™

1. Click `New Team` button on the KZ Command Node token
2. A little dialog box will pop up. Click in the text field just beneath `Enter Team Code` and paste your Data Team Roster Code. Then click `Load Team` and wait a minute. If it just hangs and shows an error in the chat box, you probably created a Kill Team in BattleScribe by accident.
3. After a moment, some boxes will appear, one for each model on your roster.
4. Each one of these boxes has a `Choose Model` button on it.
5. For each box, click the `choose model` button and then click on the appropriate model you have sitting nearby. A copy of the model will drop into the box. Hooray!
6. Once you have done this for all the boxes, click the `Finish` button on the command node dialog box
7. An orange rectangle will show up along with another dialog box. Place your models however you want in the orange box, and **make sure they are all facing the same way (towards the edge of the rectangle facing the dialog box is good)**
8. Once they are all pretty, click the `FINISH` button.
9. To avoid doing this again, drag select the Command Node and the models you just placed and save it as an object (Right Click `Save Object`).

### Get Super Fancy

You will do this part every time you play, so you technically don't need to do it now, but it is probably a good idea to practice so you get the hang of it.

1. Pick a team (click your name in the top right and select `Change Color`, then pick red or blue. Otherwise this next bit won't work I don't think. If you don't need to do this, feel free to correct this!
2. Load in the KT UI extender `Games -> Workshop`, then find `KT UI Extender`, hover to get the three dot menu, pick `additive load`
3. A fancy black mat with a bunch of buttons will show up. If you need to move the mat, you have to unlock it by right clicking on it and picking `Toggles -> Lock`. Then move it wherever you would like, then re-lock it with that same right click action.
4. Pick up your command node token, and place it on the mat on or just under the red "KT UI Extender" text.
5. Press the `Recall models` button, and all your models will arrange themselves near the token however you set them up in that orange box earlier.
6. Now click the `Extend KT UI` green button. The magic has happened.

All your models will have order tokens, and you can use the buttons on the mat to switch them all to conceal or engage. To change an individual token you can right click on the token, or right click your model and pick "engage" or "conceal". To flip a token, just click it. You can use the "Ready Operatives" button on the mat to flip all tokens back at the end of a turning point.

When your operative takes damage (or is healed) you can click on the x/x wound marker and you'll see plus and minus buttons to add or subtract wounds. Once your operative goes below 50% health, an injured token will automatically appear.

Speaking of tokens, you can now drop tokens from next to the terrain on to your model and it will float near their health and follow them around. To get rid of these tokens, just right click on them. Or maybe it's click on them. One of the two. You'll figure it out.

## KT Map Base Features

There are all sorts of things built into KT Map base: a scoreboard, ways to load missions and their objectives, showing and hiding deployment zones, tokens, dice rollers, and all sorts of good stuff. These will be added to this guide shortly. Thankfully, they are fairly self-explanatory, so just click on things that seem to make sense.

### Dice Roller

The KT Map Base has a dice rolling area.  To use it...

- Click one of the {1D, 2D, 3D, 4D, 5D, 6D} buttons to clear the rolling area of dice and to place that many dice on the rolling area.  The dice will be selected.
- Click "ROLL" button to roll the selected dice.  The dice will arrange themselves by rolled value.
- To reroll, click one of the appropriate {Low, 1, 2-, 3-, 4-, 5-} buttons to select which dice to reroll, and then click the "ROLL" button to reroll the selected dice.
  - For Ceaseless, you'll want to use the `1` button to select all the 1s to reroll.
  - For Balanced, you may want to use the `Low` button to select one lowest-valued die.
  - For Relentless, the appropriate button depends on your BS/WS.  If you have BS=3+, you'd use the `2-` button to select all 1s and 2s for reroll.
- If you used KT Command Node, you can right-click on a model and select one of its weapon profiles to roll the appropriate number of dice.


## Play the game!

Now playing is a lot easier and faster. Thanks to all the awesome people who spend a lot of time and effort making these cool tools for us!

When you are starting a game, you will follow these steps:

1. Load up the `KT Map Base` table.
2. Add some terrain via addative loading. There's a big collection of maps in the [./README.md](resources list) in this repo. When you bring in the terrain, there will be a green and red button to confirm (keep) or cancel (unload) it in case you bring in the wrong one or decide ro change your mind.
3. Bring in a `KT UI Extender` for your team via addative loading.
4. Load your kill team's `KT Command Node` saved object.
5. Plop your models onto the UI Extender mat and press the `Extend KT UI` button.
6. Play!

If you are joining someone else's game, you can skip the first two steps. Have fun!

## Some TTS/KT Interface Tips

Mousing over a model and pressing `R` will toggle distance rings of {1, 2, 3, 6} inches of the traditional colors.  You can also mouse over a model and type a digit and a distance ring of that many inches will appear.  Type `0` to hide the distance ring.

Usually after your finish a move, you should right-click on the moved model and select "Save place".  The benefit of this is so that if the model gets bumped you can right-click and select "Load place" to put the model back at the saved place.  Also great for trying out moves with confidence and ease on undoing them precisely.
