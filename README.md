# JavaScript 30 #2: CSS and JavaScript Clock

An app that gets the time from JavaScript and displays it as hands on a clock face, updated once per second.


## Key Points

The original version of this clock simply retrieved the time once per second and displayed it. The problem was that when the seconds rolled back from 59 to 0 at the top of the clock face, the seconds hand would reverse instead of incrementing forward.

This was solved by retrieving the current time once at initiation and then incrementing the seconds (once per second) after that. This way, the seconds count up indefinitely rather than ever resetting to zero. (The hours and minutes are still retrieved once per second. They do not have the same CSS transition as the second hand, which was causing this glitch.)

Just for fun, I also restyled each hand on the clock so that it would be more obvious which was which, plus a circular hub for the center axis.

I also added a conversion from the default 24-hour time to 12-hour time.


## Future Iterations

- Convert to object literal.