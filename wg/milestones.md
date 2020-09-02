Revised misson statement: Making 6 reasonably-general high-quality data stuctures thats compiles with the standards of the std to submit it to the std.

For this purpose high-quality means:
1. robust, given random data should not crash the program expect for a planned crash with a designed message.
2. Cache-aware, morden hardware has a counter-intutitive but known behavoir, data structures willfully ignorant of the basic facts are bad; I should not be.
3. Comfy user interface.

Data stucture summerys(details in seperate files):
---
1. Ring array: an array with an access pattern that loops back on itself rather then overfloawing
2. Opinionated list of lists: A array of nullable!T, where null is an end of a list.
3. Metadata: like nullable, but adds additional 7 bit int to round out the wasted space of nullable, and more flexable in useage pattern.
4. Member index arrays: A lighter version of AoSoA. Given a user defined T and a member, packes the members together for better cashe usage for searches. Highly experimental.
5. Fixed length string: When you want char[n] rather then the default char[].
6. Semi-static array: no gc, copy to larger array during overflow and custom allocator friendly array abstraction.

Month 1
----
* Get a dub package up and running
* Drasticly improve ring arrays
* Make a lazy "race" testing framework that generates documentation
* Get working reasonable quality prototypes for the other 5 data stuctures
* Learn d style and inline documention systems

Month 2
---
* Make/find a more robust testing system
* Create some sort of system for feedback that isn't std.expermental
* Improve 3 more data stuctures for feedback.

Month 3
---
* Improve remaining data stuctures.
* Finailize api and code for ring array.
* Respond to feedback.

Month 4
---
* Finailize remaining data stuctures to my own standards.
* Submit code to the std review process.
