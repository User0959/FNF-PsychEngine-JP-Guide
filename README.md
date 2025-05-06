Psych Engine (訳してサイケエンジン) の[README](https://github.com/ShadowMario/FNF-PsychEngine/blob/main/README.md)や[Wiki](https://github.com/ShadowMario/FNF-PsychEngine/wiki)などを日本語に訳しています。
もちろんフォーク大歓迎です！ Psych Engine開発チーム、そしてTHE FUNKIN CREW INCの皆様に多大なる感謝を。🔥🔥🔥❤️❤️❤️

![PsychionalEngineLogo](docs/img/PsychEngineLogoTweak.png)

Psych Engineは元々[Mind Games Mod](https://gamebanana.com/mods/301107)用に開発されたエンジンで、本家FNFの多くの問題(ラグ、入力判定)などを修正しつつ、また、プログラミングの知識を必要としないでMOD作成が行えるお手軽さが魅力のエンジンです。

## ソースコードのコンパイル方法:

[コンパイル方法](/docs/BUILDING.md)をご覧ください。

## カスタマイズオプション:

Luaスクリプトやビデオカットシーンを無効にしたい場合は、ソースコードのルートフォルダ内にある[Project.xml](https://github.com/ShadowMario/FNF-PsychEngine/blob/main/Project.xml)を開いてください。

`Project.xml`にはPsych Engineを好みにカスタマイズするための変数がいくつかあります。

まずビデオ カットシーンを無効にするには、`"VIDEOS_ALLOWED"`の行を削除するか、または`<!-- YOUR_LINE_HERE -->`のようなXMLコメントで囲んでコメントアウトするだけです。

Luaスクリプトも同じです。`LUA_ALLOWED`の行を削除するか、`<!-- YOUR_LINE_HERE -->`のようなXMLコメントで囲んでコメントアウトするだけです。

同様にLuaスクリプト、ビデオカットシーン限らずその他のカスタマイズオプションがすべて`Project.xml`ファイル内で削除、追加、編集ができます。

## lua言語・haxe言語を使ったMOD作成 (.lua/.hx)
こちらに関しては [Lua Script AIPウィキ](https://shadowmario.github.io/psychengine.lua)をご覧ください。

Lua Script AIPウィキでは212個のPlayState機能を使ったMOD作成を学ぶことができます。

## クレジット:
* Shadow Mario - メインプログラマー・Psych Engine開発チームのリーダー
* Riveren - Psych Engineのメインアーティスト・アニメーター

### スペシャルサンクス
* bbpanzu - 元チームメンバー (プログラマー)
* crowplexus - HScript Iris, Input System v3,の開発およびその他のPRs。
* Kamizeta - Psych Engineのマスコット、Pessyの作者
* MaxNeton - Loading Screen Easter Egg Artist/Animator.
* Keoiki - Note Splash Animations and Latin Alphabet.
* SqirraRNG - Crash Handler and Base code for Chart Editor's Waveform.
* EliteMasterEric - Runtime Shaders support and Other PRs.
* MAJigsaw77 - .MP4 Video Loader Library (hxvlc).
* iFlicky - Composer of Psync, Tea Time and some sound effects.
* KadeDev - Fixed some issues on Chart Editor and Other PRs.
* superpowers04 - LUA JIT Fork.
* CheemsAndFriends - Creator of FlxAnimate.
* Ezhalt - Pessy's Easter Egg Jingle.
* MaliciousBunny - Psych Engine最終アップデート(1.0)の[トレーラービデオ](https://www.youtube.com/watch?v=5VGtFyuicCg)作成

***

# Psych Engineの特徴

## Attractive animated dialogue boxes:

![Animated Dialogue Boxes](docs/img/dialogue.gif)

## New Main Menu
* A brand new menu that makes your experience even better!
![Main Menu](docs/img/MainMenu.png)

## Mod Support
* Probably one of the main points of this engine, you can code in .lua files outside of the source code, making your own weeks without even messing with the source!
* Comes with a Mod Organizing/Disabling Menu.
![Mod Support](docs/img/ModsMenu.png)


## Atleast one change to every week:
### Week 1:
  * New Dad Left sing sprite
  * Unused stage lights are now used
  * Dad Battle has a spotlight effect for the breakdown
### Week 2:
  * Both BF and Skid & Pump does "Hey!" animations
  * Thunders does a quick light flash and zooms the camera in slightly
  * Added a quick transition/cutscene to Monster
### Week 3:
  * BF does "Hey!" during Philly Nice
  * Blammed has a cool new colors flash during that sick part of the song
### Week 4:
  * Better hair physics for Mom/Boyfriend (Maybe even slightly better than Week 7's :eyes:)
  * Henchmen die during all songs. Yeah :(
### Week 5:
  * Bottom Boppers and GF does "Hey!" animations during Cocoa and Eggnog
  * On Winter Horrorland, GF bops her head slower in some parts of the song.
### Week 6:
  * On Thorns, the HUD is hidden during the cutscene
  * Also there's the Background girls being spooky during the "Hey!" parts of the Instrumental

## Cool new Chart Editor changes and countless bug fixes
![Chart Editor](docs/img/chart.png)
* You can now chart "Event" notes, which are bookmarks that trigger specific actions that usually were hardcoded on the vanilla version of the game.
* Your song's BPM can now have decimal values
* You can manually adjust a Note's strum time if you're really going for milisecond precision
* You can change a note's type on the Editor, it comes with five example types:
  * Alt Animation: Forces an alt animation to play, useful for songs like Ugh/Stress
  * Hey: Forces a "Hey" animation instead of the base Sing animation, if Boyfriend hits this note, Girlfriend will do a "Hey!" too.
  * Hurt Notes: If Boyfriend hits this note, he plays a miss animation and loses some health.
  * GF Sing: Rather than the character hitting the note and singing, Girlfriend sings instead.
  * No Animation: Character just hits the note, no animation plays.

## Multiple editors to assist you in making your own Mod
![Master Editor Menu](docs/img/editors.png)
* Working both for Source code modding and Downloaded builds!

## Story mode menu rework:
![Story Mode Menu](docs/img/storymode.png)
* Added a different BG to every song (less Tutorial)
* All menu characters are now in individual spritesheets, makes modding it easier.

## Credits menu
![Credits Menu](docs/img/credits.png)
* You can add a head icon, name, description and a Redirect link for when the player presses Enter while the item is currently selected.

## Awards/Achievements
* The engine comes with 16 example achievements that you can mess with and learn how it works (Check Achievements.hx and search for "checkForAchievement" on PlayState.hx)
![Achievements](docs/img/Achievements.png)

## Options menu:
* You can change Note colors, Delay and Combo Offset, Controls and Preferences there.
 * On Preferences you can toggle Downscroll, Middlescroll, Anti-Aliasing, Framerate, Low Quality, Note Splashes, Flashing Lights, etc.
![Options](docs/img/Options.png)

## Other gameplay features:
* When the enemy hits a note, their strum note also glows.
* Lag doesn't impact the camera movement and player icon scaling anymore.
* Some stuff based on Week 7's changes has been put in (Background colors on Freeplay, Note splashes)
* You can reset your Score on Freeplay/Story Mode by pressing Reset button.
* You can listen to a song or adjust Scroll Speed/Damage taken/etc. on Freeplay by pressing Space.
* You can enable "Combo Stacking" in Gameplay Options. This causes the combo sprites to just be one sprite with an animation rather than sprites spawning each note hit.


#### Psych Engine by ShadowMario, Friday Night Funkin' by ninjamuffin99
