You looked for and clicked on not one, but **TWO** readme files? Your dedication impresses me. 

Because this program is so bad, you need to do a lot of setup before it can work. In that time, you might as well read all the txt files and process them manually.  But if you really have nothing better to do with your time, then you can read these setup instructions. 
1. Download this entire repository. If you do it right, then one of your computer's attack stats should go up. 
2. If you already have Eclipse, then open Eclipse and open this project in Eclipse. 
3. Find Commands.java in this project. Type your commands in the commands() method. Click run. Wait for the commands to execute. 

2. If you don't already have Eclispe, then install Eclipse. It's free, but specific instructions will depend on your computer. If you have problems, then just Google your error messages and click random results until the problem goes away. 
3. Open Eclipse and click "Launch". 
4. There should be a "File" button in the top left corner. Click that, then click "Open Projects from File System...", then click "Directory". 
5. Find your downloaded repository. At this point, it's probably in your "downloads" folder. Click the folder that contains it, and then click "Finish". 
6. Click the "Window" button that should be a little to the right of the "File" button. Click it. Then click "Perspective", "Open Perspective", and "Java". If you don't see the "Java" button in that menu, then you can skip this step. 
7. On the left sidebar, you should see "DataSeek". Click the ">" next to it, then click the ">"s next to "src" and "notDefault". 
8. Double-click "Commands.java". Type whatever commands you want in the first method (between "commands() {" and "}"). Click the run button (green circle with right triangle in top bar). Wait for the commands to execute. 
If I tell you to click a button and you can't find it, then you can try sending me a screenshot of what your screen looks like right before you were told to click that button. 

This program uses Java, so when you type the name of a command, you need to type (""); right after the command's name and put your input between the quotes. For example, if you wanted to execute the ds command on movepool>=128,!learnsalltypes , then you'd have to type 

ds("movepool>=128,!learnsalltypes");

When you want to put multiple inputs into a command, separate them with ",". Specific instructions for each command are in the Commands.java file. 

The ds, dt, and mean commands deal with Pokemon data. Currently, the only information I have on each Pokemon are their moves, the size of their movepools, whether or not they can learn each type of move, and each of their base stats, and their base stat totals. You should probably tell me if you really want this program to read something else. 

All Pokemon information is divided into two categories: statistics and truths. Statistics are numbers, and truths are yes-or-no questions. "Can it learn karate chop?" and "Can it learn a fire move?" are both examples of truths. "What is its special defense?" and "How many types of movex can it learn?" are examples of statistics. 

When using ds to search truths, you only need to type the name of the truth. For example, ds("karatechop"); searches for Pokemon that learn karate chop. You can type "!" in front of the truth, but only if you want to find Pokemon where that truth is false. 

When using ds to search statistics, you need to not only type the statistic's name, but also one of =, <, >, !=, <=, or >= and a number. For example, /ds("movepool<8"); searches for Pokemon that learn less than 8 moves. 

dt takes both statistics and truths. It only takes their names, no need for =, >, or any of that crap. It prints numbers for statistics and either "true" or "false" for truths. 

When using mean, the thing before the first "," must be the name of a statistic. Everything after that is read the same way as ds. 
