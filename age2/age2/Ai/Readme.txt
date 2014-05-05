Slak_BotTC
Version 0.9.3
Author: Dan Cieslak <slak96@yahoo.com>
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=

This is my first attempt at a custom AI.  As it is
a 0.9.x release, it is not a final release (yet).
I decided to release it to get some more feedback
for it.

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
What Slak_bot does:
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
Slak_bot has been improved and modified to play
the expansion pack.  It will play the new civs
pretty well!

Slak_bot's basic design principle is to get to
Imperial reasonably quickly.  It deals quite well
with booming AIs.  It does not handle rushes very
well, though will generally fend off BingAI-3.1,
it will be crushed by Maccha Version 5.  Future
releases may attempt to deal with this shortcoming.

Furthermore, the military for each civilization
is unique.  Thanks to Michael D. Eschner (MDE)
for inspiration and many of the unit mixes.

Slak_bot will build "response" units 20% of the
time.  The response unit is determined based on
what is attacking Slak_bot (for example: it will
build skirmishers to counter archer units).
Response unit selection is also customized for
each civilization (though some are identical).

Slak_bot's navy is pretty standard.  The only
customization is for the Vikings (Longboats
instead of Fireships).  The British lack of
cannon galleons is not factored into ship
production.

Slak_bot now uses escrow.  Resources in escrow
are generally used for research or important
buildings.  Thanks to Bingmann for his help.

Slak_bot is best used in default resource,
random map, Dark-age start game.  It may 
play other settings, but I doubt it will play
them very well.

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
What Slak_bot does not do:
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
SLAK_BOT DOES NOT RESOURCE CHEAT!  There are 
no references to any of the cc-* directives.
It does reference players-military-population
(which the documentation claims is "the
equivalent of a human player checking the
timeline").  If I could, I would have 
implemented it using players-unit-count and
players-unit-type-count (both of which rely
only upon units that the AI has seen).  But,
there is no "soldier-line"-type parameter
and coding cases for each of the different
unit lines is just impractical.

Slak_bot does not even try to build a wonder.

Slak_bot also does not research various
items, mostly tower technologies.  Priority
is given to a civ's "strength" or if the
appropriate units are fielded.

The forward building placement has been greatly
improved (See Maccha Version 5) under the
expansion pack.  Sadly, Slak_bot does not make
use of this.  In fact, it is very difficult to
detect and deal with a rush.  I spent a lot
of time trying, and was not very successful.
I have two final ideas, but may not have the time
to implement them.

I have given up on walls.  The wall-placement
code doesn't understand that forrests can (and
do) disappear over time.  This leads to holes
in the wall.  Pointless, I say.  Plus, it wastes
a lot of villager time.  And since the tactical
AI seems to favor towers, I'd rather spend the
resources on something that kills.

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
Bugs (in an almost priortized list):
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
* Villagers do not colonize other islands.
* Testing higher population games.
* Town sizes on "watery" maps.
* Boat booming is pretty weak.
* Slak_bot does not ask allies for tribute.
* Slak_bot does not respond to requests for tribute.
* Slak_bot may have trouble in prolonged games.
* Add forward building.
* Add Non-Dark-age start support.
* Put excess stone to use.
* Prevent fishing boat scouting.

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
Acknowledgements:
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
This AI was influenced by the Petersen's (AoK's
default AI),  Michael D. Eschner's (MDE_Land_Aggro),
Bingmann's (BingAI 2.2) and Doug Brucks' 
(Doug's Test AI).  MDE has a good economy and
I really liked the combined arms.  Bingmann
gave me the idea to leap imperial, though I
progress a bit slower than his.  Brucks' has
a good attack response system.  MDE's AIs are
under Gnu Public License (GPL) and I have his
permission to use limited portions of his code
as I see fit.  Bingmann's AI appears to be in
the public domain, but I didn't use anything
of his aside from the idea of advancing quickly
to Imperial.  I could not find copyright information
on Brucks' AI, so I assume it is free for use
provided credit is given.  Credit is duely given.
Unless otherwise noted, I developed the rest of
the AI.  Any similarities to any other code
(fictional, alive or dead) is purely coicidental.
All spelling errors are my own.  This code is
being provided under a BSD-style license (included
at the end of this file).  Essentially, you may
use it, provided you give me credit in any
derivative work.  If it should be included in
something advertised for sale, you must include
the following acknowledgement:

This product includes software developed by Dan
Cieslak.

Furthermore, my name cannot be used to endorse
or promote the product without written permission.

-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
Copyright and License
-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=
Copyright 1999-2000, Dan Cieslak  All rights reserved.
Available under BSD-like license:

Redistribution and use in source and binary forms, 
with or without modification, are permitted provided 
that the following conditions are met: 

Redistributions of source code must retain the above 
copyright notice, this list of conditions and the 
following disclaimer. 

Redistributions in binary form must reproduce the 
above copyright notice, this list of conditions and 
the following disclaimer in the documentation and/or 
other materials provided with the distribution.

All advertising materials mentioning features or 
use of this software must display the following 
acknowledgement:
 
This product includes software developed by Dan Cieslak.

The name of Dan Cieslak may not be used to endorse 
or promote products derived from this software 
without specific prior written permission. 

THIS SOFTWARE IS PROVIDED BY DAN CIESLAK "AS IS" AND 
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT 
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY 
AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. 
IN NO EVENT SHALL DAN CIESLAK BE LIABLE FOR ANY DIRECT, 
INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR 
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, 
PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF 
USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) 
HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, 
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT 
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY 
OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE 
POSSIBILITY OF SUCH DAMAGE.
