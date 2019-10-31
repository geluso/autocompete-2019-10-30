## AutoCompete 2019-10-30

### Start Your Engines!
Here's a problem to make sure you're on board and chugging along correctly.
Read one line in a file and sum the total of all digits added together. Print
out the total.

Write a problem called `sum` that reads the single line of input and prints
the sum of the digits.

* Sample Input: `12345678998765432123456789876543213`
* Sample Output: `173`


### Candy Mountain
There's an island in the Bermuda Triangle where it pours down candy from the
sky. It pours down so much candy candy fills every valley across the island.
What overflows from the valleys rolls off and sinks in to the sea.

Write a program called `candy_mountain` that reads height information of
mountains and valleys on the island and returns the total area of island
covered in candy. The height information comes in as one line of digits.  You
can assume the height info starts and ends with a zero, and each height will
be a single digit.

Given the height information below you can see the candy pool up so it's level
filling each valley. There are five valleys on this island and they fill up
with 1 piece of candy, 6 pieces, 9 pieces, 5 pieces and 3 pieces respectively
for 24 pieces of candy filling valleys across the whole island.

```
        8
        7   7
        6   6
        55  5  5
        444 44 4 4
   3   3333333 3 33
   2   2222222 2 222
 1 111111111111111111
0000000000000000000000
```

```
         (9)    
             (5)
        8
        7***7  (3)
    (6) 6***6
 (1)    55**5**5
        444*44*4*4
   3***3333333*3*33
   2***2222222*2*222
 1*111111111111111111
0000000000000000000000
```

1 + 6 + 9 + 5 + 3 = 24

* Sample Input: `010311138543741543210`
* Sample Output: `24`

### Mummies in a Pyramid
Write a program called `pyramid` that reads a single integer from standard input  
then print out a pyramid (using asterisks) that encloses mummies (using $ symbol)  
Mummies should never be outside or on the edge of the pyramid.  
Tests will run against integers from 1-100 inclusive

Sample Input: `1`  
Expected Output :
```
*
```

Sample Input: `2`  
Expected Output :
```
 *
***
```


Sample Input: `3`  
Expected Output :
```
  *
 *$*
*****
```


Sample Input: `4`  
Expected Output :
```
   *
  *$*
 *$$$*
*******
```

Sample Input: `5`  
Expected Output :
```
    *
   *$*
  *$$$*
 *$$$$$*
*********
```

### Haunted Elevator

The Haunted Elevator belongs to a building that has no basement and will always start on floor 1.  
The first elevator press will move the elevator in the desired direction by 1 floor.  
If the elevator is on floor 1 and wants to go DOWN one step, the elevator is still on floor 1.  
The Haunted Elevator will reverse the direction after every other button press.

If the elevator never got haunted here is how it would react to someone pressing UP DOWN UP

- The elevator starts at floor 1
- Pressing UP moves the elevator from floor 1 to floor 2
- Pressing DOWN moves elevator from floor 2 back to floor 1
- Pressing UP moves the elevator from floor 1 to floor 2

But, that's not how things go. This elevator gets haunted every other time the button is pressed.
When the elevator is haunted it goes in the opposite direction of the button that's pressed.

- The elevator starts on floor 1 and is not haunted.
- Pressing UP causes the elevator to go from floor 1 to 2. It is now haunted.
- Pressing DOWN causes the haunted elevator to go from floor 2 to 3 and now it is not haunted.
- Pressing UP causes the un-haunted elevator to go from floor 3 to floor 4.
- The elevator went from floor 1 to floor 4 for a total of 3 floors.

Parse each line of button presses, return the resulting floor that the elevator lands on, on it's own line.

Sample Input: `UP DOWN UP` will go UP 3 floors.  
Expected Output: `3`  

Sample Input: `DOWN UP UP UP DOWN`  
Expected Output: `1`  

Sample Input:
```
UP UP UP
UP UP DOWN UP UP
UP UP DOWN DOWN UP UP UP
```
Expected Output:
```
2
2
3
```

### Ghostbusters

Ghosts have invaded our city!

Find all ghosts that are inside buildings, and remove them!

Read the ascii art of a city skyline from standard input to reproduce the ascii buildings.  
Print out the same buildings without any Indoor Ghosts  
and with all Outdoor Ghosts left intact

Ghost positions use the `@` symbol

Sample Input:
```
                        +
    @                   |
                   +---------+                @
                  +  @  @     +             +------+
          @        +---------+         @    |     -+    @
      @             @  | |                  |     @|
+-----------+  +-----+ | |    @             |      |
|           |  |     | | |                  |   ---+
|  @     ---+  | @   | | | @               @|      +-------+
+------- @  |  |     | | |   +-----------+  |      |       |
| ----------+  | ----+ | |   |          @|  | -----+ @     |
|           |  |     | | |   +-----------+  |      |       |
|    @      | @|     | | |   |          @|  |      |       |
+-----------+  +---  | | |   +--------   |  |      |       |
|           |  |     | | |   |@          |  |      |    @@ |
|          @|  |     | | |   |           |  +----  |       |
+-----------+  +-----+ +-+   +-----------+  +------+-------+
```

Expected Output:
```
                        +
    @                   |
                   +---------+                @
                  +           +             +------+
          @        +---------+         @    |     -+    @
      @             @  | |                  |      |
+-----------+  +-----+ | |    @             |      |
|           |  |     | | |                  |   ---+
|        ---+  |     | | | @               @|      +-------+
+-------    |  |     | | |   +-----------+  |      |       |
| ----------+  | ----+ | |   |           |  | -----+       |
|           |  |     | | |   +-----------+  |      |       |
|           | @|     | | |   |           |  |      |       |
+-----------+  +---  | | |   +--------   |  |      |       |
|           |  |     | | |   |           |  |      |       |
|           |  |     | | |   |           |  +----  |       |
+-----------+  +-----+ +-+   +-----------+  +------+-------+
```

You can visit https://tinyurl.com/hackoween-ghostbusters for a copy-n-pastable city input.


### superNATURALcase and spooKycaSe

superNATURALcase words are written with alternating all-caps and all-lowercase formats, starting with lowercase, and no other space separators.

spooKycaSe words are written with each second-to-last letter being uppercased, and no other space separators.

Read each line from standard input.  
Each line of text will be either superNATURALcase or spooKycaSe.

Print out the same lines with text transformed to Sentence case.  
Keep all punctuations as is.

Sample Input:
```
whatSHAPEwasTHISwhoCAMEtoUS,
withBASILISKeyesSOominous,
wiThmouThSosweEt, SopoisonoUs,
andTORTUREDhandsSOpale?
WesAwhErwaveriNgToaNdfRo,
throuGhdaRkaNdwiNdWesAwhErGo;
yetWHATherNAMEwasDIDnotKNOW;
aNdfeLtoUrspiriTsfaIl.
```

Expected Output:
```
What shape was this who came to us,
With basilisk eyes so ominous,
With mouth so sweet, so poisonous,
And tortured hands so pale?
We saw her wavering to and fro,
Through dark and wind we saw her go;
Yet what her name was did not know;
And felt our spirits fail.
```

_credit: “The Vampire” by Conrad Aiken_

### Poker
Write a program called `poker` that reads five lines representing cards
and returns a description of the type of hand.

Your program should print out one of the following descriptions depending on
the hand:

* "bunk" - when there are no matches
* "one pair" - when there are only two cards of the same value
* "two pairs" - when there are two pairs of different cards with the same
  value (3, 3, 4, 4)
* "three of a kind" - when there is three of one value 
* "four of a kind" - when there is four of one value
* "full house" - when there is three of one value and two of another
* "straight" - when all five cards are consecutive (twos are low, aces are
  high, [8, 9, 10, J, Q] is a straight)
* "flush" - when all cards have the same suit
* "straight flush" - when all five cards are the same suit and are consecutive
  values
* "royal flush" - when all five cards are the same suit and the cards are
  specifically [10, J, Q, K, A]

The input will be five lines describing the cards in the hand:

```
two of spades
two of clubs
three of hearts
three of diamonds
three of diamonds
```

Sample Output: `full house`

#### Code Golf
Write a program called `golf` that reads in the position of a golf ball and a
hole and a list of trajectories. 

The trajectories representing hitting the ball. Just add the trajectories to
the current position of the ball. Do not try to simulate "rolling along the
path." Stop the program when the ball is in the same position as the hole and
print out how many shots it took to get there.

Sample Input
```
ball <0,0>
hole <15,20>
<5,5>
<7,5>
<3,8>
<0,2>
<1,1>
<-2,1>
```

* <5,5> the ball moves from <0,0> to <5,5>
* <7,5> the ball moves from <5,5> to <12,10>
* <3,8> the ball moves from <12,10> to <15,18>
* <0,2> the ball moves from <15,18> to <15,20>
* The ball is in the hole in four shots!
* Ignore the remaining trajectories.

Sample Output
```
Hole in 4
```
