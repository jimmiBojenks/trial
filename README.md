# Warning: This is no longer an open source project!

You can still [play the game for free](http://www.basketball-gm.com/), but it's no longer open source. If you want to know why, [read the explanation here](http://www.reddit.com/r/BasketballGM/comments/1sarll/open_source/). I'm leaving the source code for the last open source version here, but it won't be updated even as Basketball GM continues to evolve.



## Basketball GM 3.2.0

A single-player basketball simulation game. Make trades, set rosters, draft
players, and try to build the next dynasty, all from within your web browser.
The game is implemented entirely in client-side JavaScript, backed by
IndexedDB.

* Website: http://www.basketball-gm.com/

* Development website: https://github.com/jdscheff/basketball-gm

* Main developer: Jeremy Scheff <jdscheff@gmail.com>



### License

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU Affero General Public License version 3 as published by
the Free Software Foundation.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU Affero General Public License for more
details.

You should have received a copy of the GNU Affero General Public License along
with this program.  If not, see <http://www.gnu.org/licenses/>.



### Installing and Running

If you just want to play the game, go to http://www.basketball-gm.com/
Instructions below are for developers who want to run a copy so that they can
test changes to the code locally.

To run the game with local files, you need some way of running a web server to
display the content. There are currently three ways to do it. It doesn't matter
which you use as long as you can get it to run on your computer.



#### 1. Mongoose - Easiest on Windows

Run `mongoose-tiny-4.1.exe`. Point your browser to http://localhost:8080/

That's it.

If that doesn't work, try right clicking on the Mongoose icon in your
notification area and poke around in there. You can also see if there is a
newer version of Mongoose available http://cesanta.com/downloads.html 



#### 2. web.py - Easiest on Linux

Install Python and web.py (as simple as `sudo apt-get install python-webpy` on
Ubuntu). Then, from the command line, run:

    python runserver.py

Point your browser to http://localhost:8080/

If that URL doesn't work, try http://0.0.0.0:8080/



#### 3. Apache

If you can't get one of the above methods to work, the mod_rewrite rules in
`.htaccess` can be used to make Apache run Basketball GM. Everything should work
if you just have a domain/subdomain point at this folder with mod_rewrite
enabled.



### Debugging and Problem Solving

For debugging information, go to http://play.basketball-gm.com/ and click on
Help > Debugging.

To run the test suite, go to http://localhost:8080/test
