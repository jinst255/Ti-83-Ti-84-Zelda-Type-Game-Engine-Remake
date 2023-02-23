# Ti-83-Ti-84-Zelda-Type-Game-Engine-Remake
Zelda Type Game Engine Remake. This is not so much a game as an engine. And Nintendo if you care go after Oiram first.

Remember that this is done on a calculator, and programed entirely in TI-basic. Don't expect too much.

Original engine design take from Timothy J Swan. You can find his first zelda video on his channnel here:
https://www.youtube.com/watch?v=KMMgo7NVDN8&list=PLymYmaupkVCckzGUtMMuIqex9b8-CqgYf 

I redesigned and optimized as much of it as I could.
Drawing walls and other objects to the screen is WAY faster, with my calc I estimate speeds of up to 600% faster. (6x faster). This is accomplished by only drawing the objects that are placed on the screen.  And not drawing any spaces “ ”.

In order to use this speed you must add “1→D:Goto D3” to the end of your “If O=0 and N=0” statements.
You must also put you map data into matrix A, and then run the program “FASTMAP”. This will return ⌊Y, ⌊X, and ⌊T. Then recall these into your program under your “If O=0 and N=0” statements. 

To put your map data into Matrix A do the following:
{8,16}→dim([A]
Then
Fill(0, [A])
You do not need a program to run these, you can do it all on the home screen.
After you have created [A] and filled it with zeros you can edit it. Go to the matrix menu and click left and then enter. This is set you up to edit matrix A.
Here are the objects that this engine is currently calibrated to print to the screen: (Stuff you can add to your map data)
0=Space “ “ (This will not get printed)

1=Wall “O”

2=Door “D”

3=Fake wall “O” (Looks like a wall but the player can walk through it)

4=Grass/Bush “G” 

5=Sign “P” (Just a sign that can show you text, without having to redraw the screen)

6=Chest “▫” (Not fully implemented)

7=Person “π” (Can talk to you without having to redraw the screen)

8=Save point “S” (Saves player data to be recalled next time the program is run)

9=Item (Note that you can pick up an item and it is added into your inventory in the correct slot and quantity (1). BUT, if you user walks of screen and back on it will be there again)

10=Path “•” (Just a path)





I also made major improvements to player speed. 
I will not be covering how I did this, but you can clearly see the differnce here:
https://user-images.githubusercontent.com/73206799/221057483-198cb708-efd4-4fcf-bd9c-1f53bd6ad373.mp4





FINAL NOTE: 
In order to run this you will have to ungroup it. (2ND, “+”, up, “ENTER”, go to ZEL, “ENTER”).

There is a lot more I could add in this readme, I probably will not get around to adding them into this readme.
