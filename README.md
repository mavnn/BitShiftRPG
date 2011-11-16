# Core Mechanics

Abilities in Bit Shift are represented by a Shift (can be positive or negative) and a level between 10 and 20. This is represented as Shift/Level.

Normals humans tend to be rated as 0/15.

If an ability increases, raise the Level by one. If that would take you to level 21, increase the shift by one and drop the Level to 10.

If an ability decreases, drop the level by one. If that would take the level to 9, drop the shift by one and raise the Level to 20.

To calculate a 'result', roll two d10 which you've marked as being positive and negative. Add the positive dice and subtract the negative. If your target number (or opponent) is the same shift as you, you're done. If not:

* Take the result with the lower shift. Half it (rounding up!). This is the effective result at the next shift level.
* If the effective result is still at a lower shift than the opposing result, repeat until both are at the same shift (the effective result will never drop below one, so if it reaches one just count that as the result)
* The 'Effect Shift' (only needed on rolls where the level of success matters) is the number of times the higher result can be halfed (rounding up) before it is the same or smaller than the lower result.

Example:

Bob tries to hit Bill with a skill of 2/13 (Bob is very, very good at unarmed combat). Bill frantically attempts to block with his untrained skill of 0/15.

Bob rolls +8, -2 for a result of 2/21. Bill rolls +3, -4 for a result of 0/14. Bill's effective result is:

* 1/7 (14/2) at shift 1
* 2/4 (7/2, rounded up) at shift 2, the same shift as Bob's roll.

Hitting somebody can have varying levels of success, so we also calculate the Number of shifts of success:

* 21/2 is 11 (giving one shift)
* 11/2 is 6 (giving two shifts)
* 6/2 is 3, which is lower than Bob's effective result.

Bob connects with two shifts of success, a remarkable result that will give a large bonus to his damage roll.


# Design goals

Obviously, there's not a whole lot going on here yet. But this is the list of goals that I'm looking to cover.

## Scalable

Many RPGs cover a specific ability range very well, but fail badly when characters or events push the limits of thier scale. Wookie's in WEGs Star Wars bouncing blaster bolts off their chests is a classic example.

Bit Shift deals with this by scaling ability in 'Shifts' and having easy conversions between them: if Bob is twice as strong as Bill, it doesn't matter if Bob and Bill are superheroes throwing buses around, or fairies waving pins at each other. Bob's advantage in either case has exactly the same impact on any contest between them.

## More than physical

Rule sets like Pendragon brought into RPGs the idea that characters could be represented by the strengths and weaknesses of their character and goals as well as their skills and abilities. Bit Shift will incorporate the idea that (for example) you can push your abilities further defending your true love than in a friendly sparring match.

## Unified rules

The ruleset should be of minimal size, and as much as possible should be based around the same small set of core mechanics.

## Classless

Nothing wrong with classes, I just don't like them.

## Interactive

Ideally I want to avoid the classic "roll iniative and then wait your turn" of most RPGs. Rivers and Lakes was great at avoiding this.

## Software support

I need some to keep my hand in on GUI development and would like to look a bit more into machine learning. As such, character generators and GMs aids (especially tools for running large numbers of Mooks) are likely to appear at some point.

# License

<a rel="license" href="http://creativecommons.org/licenses/by/3.0/"><img alt="Creative Commons Licence" style="border-width:0" src="http://i.creativecommons.org/l/by/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">Bit Shift RPG</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://mavnn.co.uk" property="cc:attributionName" rel="cc:attributionURL">Michael Newton</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/3.0/">Creative Commons Attribution 3.0 Unported License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/mavnn/BitShiftRPG" rel="dct:source">github.com</a>.