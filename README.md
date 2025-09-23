# Micro:Bit Arcade Code Club RoadMap 2025/26

To enable students in Years 4–5 to design, code, and test a simple arcade-style game using the BBC Micro:bit, while developing computational thinking, problem-solving, and digital creativity skills.

---

## **Learning Goals**
By the end of year, student will:
  - Understand key programming concept: Sprite, Controller, game, Math etc.
  - Use MakeCode to Code Microbits and control Arcade
  - Create a working game for food and enemy and collect coins
  - Test, Debug and redefine code

  - --

  ## **Weekly Plan**

  | **Week** | **Category**      | **Key Concepts**           | **MakeCode Blocks**                            | **Basic Python (MicroPython) Code**                                                                                                                                                 | **Learning Outcome**                        |
| -------- | ----------------- | -------------------------- | ---------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| **1**    | Sprites           | Create game characters     | `sprites.create()`                             | `python<br>player = game.create_sprite(2, 4)`                                                                                                                                       | Students create and place sprites on screen |
| **2**    | Controller        | Control sprite with inputs | `on button A pressed`                          | `python<br>def on_button_a():<br>&nbsp;&nbsp;&nbsp;&nbsp;player.move(-1)<br>input.on_button_pressed(Button.A, on_button_a)`                                                         | Move sprite left/right with buttons         |
| **3**    | Game              | Game start/end, restart    | `game.over()`, `restart`                       | `python<br>game.game_over()`<br>`python<br>control.reset()`                                                                                                                         | Game ends on condition and can restart      |
| **4**    | Music             | Play sound on events       | `play sound`, `start melody`                   | `python<br>music.play_tone(262, music.beat(BeatFraction.WHOLE))`                                                                                                                    | Add sound when events occur                 |
| **5**    | Scene             | Set background, camera     | `set background color`, `camera follow sprite` | *Not all scene functions available in MicroPython*                                                                                                                                  | Visual environment setup                    |
| **6**    | Info              | Score, lives, timers       | `change score`, `set life`                     | `python<br>info.change_score_by(1)`<br>`python<br>info.set_life(3)`                                                                                                                 | Track score/lives and countdowns            |
| **7**    | Loops             | Repeat actions             | `forever`, `repeat`                            | `python<br>while True:<br>&nbsp;&nbsp;&nbsp;&nbsp;basic.pause(1000)`                                                                                                                | Run repeating actions                       |
| **8**    | Variables         | Store values like score    | `set`, `change`                                | `python<br>score = 0<br>score += 1`                                                                                                                                                 | Control values in the game logic            |
| **9**    | Math              | Use operations, randomness | `pick random`, `+`, `-`                        | `python<br>import random<br>x = random.randint(0, 4)`                                                                                                                               | Random positioning or speed                 |
| **10**   | Animation         | Animate sprites            | `run animation`, `pause`                       | *Animations are limited in MicroPython; simulate via images:*<br>`python<br>images = [Image.HEART, Image.HAPPY]<br>for img in images:<br>&nbsp;&nbsp;&nbsp;&nbsp;display.show(img)` | Animate characters or effects               |
| **11**   | Arrays (Optional) | Store lists of values      | `create array`, `add value`                    | `python<br>enemies = [1, 2, 3]<br>enemies.append(4)`                                                                                                                                | Manage lists of objects                     |
| **12**   | Text Functions    | Show messages              | `show string`, `splash`, `join`                | `python<br>display.scroll("Score: " + str(score))`                                                                                                                                  | Show custom messages to player              |

## **Key Concepts**

- Understand event driven programming
- Create custom blocks in MakeCode to keep code organized
- Building testing and improving projects step-by-step

## **Resources**
- [make code for Micro:bit](https://arcade.makecode.com/)

- --
This roadmap is designed to be flexible - adjust pace and content based on students progress and interest.
