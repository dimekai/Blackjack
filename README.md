# Blackjack

It also known as 21, is a card game where players try to get as close to 21 points as possible without going over. This program uses images draw with the text characters, called _ASCII art_. The playing cards in this program are an example of _ASCII art_:

```
 ___   ___
|A  | |10 |
| ♣ | | ♦ |
|__A| |_10|
```

## How works?
**Rules**
1. Try to get as close to 21 without going over.
2. Kings, Queens, and Jacks  are worth 10 points.
3. Aces are worth 1 or 11 points.
4. Cards 2 through 10 are worth their face value.

(H)it to take another card
(S)tand to stop taking cards.

On your first play, you can (D)ouble down to increase your bet but mus hit exactly one more time before standing

In case of a tie, the bet is returned to the player.
The dealer stops hitting at 17.

## Example
```
Rules
    1. Try to get as close to 21 without going over.
    2. Kings, Queens, and Jacks are worth 10 points.
    3. Aces are worth 1 or 11 points.
    4. Cards 2 through 10 are worth their face value.
    
    (H)it to take another card
    (S)tand to stop taking cards.

    On your first play, you can (D)ouble down to increase your bet but mus hit exactly one more time before standing

    In case of a tie, the bet is returned to the player.
    The dealer stops hitting at 17.
    
Money: 5000
How much do you bet? (1 - 5000, or QUIT)
```
- **When you win**
  ```
    How much do you bet? (1 - 4925, or QUIT)
    > 900
    Bet: 900

    DEALER: ???
     ___   ___
    |## | |K  |
    |###| | ♦ |
    |_##| |__K|

    PLAYER: 20
     ___   ___
    |K  | |Q  |
    | ♠ | | ♠ |
    |__K| |__Q|


    (H)it, (S)tand, (D)ouble down> S 
    Dealer hits...

    DEALER: ???
     ___   ___   ___
    |## | |K  | |J  |
    |###| | ♦ | | ♥ |
    |_##| |__K| |__J|

    PLAYER: 20
     ___   ___
    |K  | |Q  |
    | ♠ | | ♠ |
    |__K| |__Q|


    DEALER: 26
     ___   ___   ___
    |6  | |K  | |J  |
    | ♦ | | ♦ | | ♥ |
    |__6| |__K| |__J|

    PLAYER: 20
     ___   ___
    |K  | |Q  | 
    | ♠ | | ♠ |
    |__K| |__Q|

    Dealer busts! You win $900!
    Pres Enter to continue...
    Money: 5825
    ```
- **When you lost**
    ```
    How much do you bet? (1 - 6625, or QUIT)
    > 700
    Bet: 700

    DEALER: ???
    ___   ___
    |## | |2  |
    |###| | ♦ |
    |_##| |__2|

    PLAYER: 15
    ___   ___
    |A  | |4  |
    | ♣ | | ♣ |
    |__A| |__4|


    (H)it, (S)tand, (D)ouble down> S
    Dealer hits...

    DEALER: ???
    ___   ___   ___
    |## | |2  | |K  |
    |###| | ♦ | | ♥ |
    |_##| |__2| |__K|

    PLAYER: 15
    ___   ___
    |A  | |4  |
    | ♣ | | ♣ |
    |__A| |__4|

    Press Enter to continue...

    DEALER: 19
    ___   ___   ___
    |7  | |2  | |K  |
    | ♣ | | ♦ | | ♥ |
    |__7| |__2| |__K|

    PLAYER: 15
    ___   ___
    |A  | |4  |
    | ♣ | | ♣ |
    |__A| |__4|

    You lost!
    Pres Enter to continue...
    Money: 5925
    ```
- **When you are tie**
    ```
    How much do you bet? (1 - 4925, or QUIT)
    > 1500
    Bet: 1500

    DEALER: ???
     ___   ___
    |## | |2  |
    |###| | ♥ |
    |_##| |__2|

    PLAYER: 19
     ___   ___
    |10 | |9  |
    | ♦ | | ♣ |
    |_10| |__9|


    (H)it, (S)tand, (D)ouble down> S
    Dealer hits...

    DEALER: ???
     ___   ___   ___
    |## | |2  | |J  |
    |###| | ♥ | | ♦ |
    |_##| |__2| |__J|

    PLAYER: 19
     ___   ___
    |10 | |9  |
    | ♦ | | ♣ |
    |_10| |__9|

    Press Enter to continue...

    DEALER: 19
     ___   ___   ___
    |7  | |2  | |J  |
    | ♠ | | ♥ | | ♦ |
    |__7| |__2| |__J|

    PLAYER: 19
     ___   ___
    |10 | |9  |
    | ♦ | | ♣ |
    |_10| |__9|

    It's a tie, the bet is returned to you
    Pres Enter to continue...
    Money: 4925
    ```

> **Note**: _The card suit symbols do not exist on your keyboard, which is why we call the `chr()` function to create them. The integer passed to `chr()` is called a Unicode _code point_, a unique number that identifies a character according to the Unicode standard_.

**Tags**: `large` `game` `card game`.

