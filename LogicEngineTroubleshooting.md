#some common problems encountered with the Logic Engine

I'm going to try and document some problems that builders have come across with the first run of RSeries Logic Engines. You can always email me at joymonkey @ gmail.com , but have a look here first to see if there's a documented fix for you.


# Only 1 Front LED Board is Working #
Problem: You've chained up both Front LED boards to the AVR board and only the first board is lighting up.

![https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/fld-connections_th.png](https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/fld-connections_th.png)
## Test Both Boards ##
We've got two LED boards; one with IN and OUT pins (the Master) and one with just a set of IN pins (the Slave). First make sure both boards are working on their own. Connect them to the AVR board in turn like this...

![https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/trouble/test-fronts.png](https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/trouble/test-fronts.png)

Chances are that both boards are working fine. The problem

## Check the Master OUT ##
Hook everything up like this and test for 5V at the end.

<a href='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/trouble/joshimus.png'><img src='https://rseries-open-control.googlecode.com/svn/trunk/Media/Misc/LEwiki/trouble/joshimus_th.png' /></a>

If you do have 5V, then it's the OUT pin on the master board that's the problem.

## Make the Slave a Master ##
We can solder pins onto the Slave board and use that as the Master board instead. You'll need a 3-pin 90 degree pin header (like <a href='https://www.sparkfun.com/products/553'>this</a>). Solder it onto the Slave board similarly to how its placed on the Master board. Plug everything back in using that board as your new Master and (fingers crossed) all should be well.

## Clean Up The Master OUT ##
If you're pretty comfortable soldering and have some solder braid (aka solder wick) on hand you can try repairing the shoddy solder joint on that OUT pin. Let the iron heat up as much as possible, then tin the tip of the iron with some solder like <a href='http://youtu.be/Rm28jkKGMz4?t=54s'>this</a>. Put the braid on the solder that's on the troublesome OUT pin, then hold the soldering iron onto the braid so some of the old solder 'wicks' into the braid (like <a href='http://youtu.be/BrAJpz9Mdm4?t=2m17s'>this</a>) - be careful not to hold it there for more than two seconds and try not to put too much pressure on it (we don't want to damage the thru-hole). With the solder joint cleaned up like that, test the whole thing out again. If we're lucky the problem should have fixed itself. If not, give it another try, adding a tiny bit more solder to the joint to get things flowing.

