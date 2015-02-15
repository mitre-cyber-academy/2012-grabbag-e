README 
Binary/Reverse Engineering 300 - The Esoteric Challenge. 

Universal dependencies: 
Piet interpreter- I used npiet (http://www.bertnase.de/npiet/) (Version 1.3 required)
Ook interpreter - I simply used the online js version http://www.netteleuthe.de/gc/ook/

Rebuild: 
In order to rebuild this challenge the following dependencies are required: 
Perl 
Perl Parse::RecDescent: can be installed with cpan Parse::RecDescent
PnmtoPng can be install on Windows with the GNU windows tool

Testing Solution: 
There are two ways to test this challenge, the first is to just use the answer script that I've provided (answers.txt in the Solutions Folder), and the second is to use the solution script for the first three challenges and edit the picture for the second part (which is the expected solution for the challenge) 
	
First Solution. 
	Add npiet to your path and move the answers.txt to the same folder as the Binary-300.png challenge picture. 
	run the command "npiet Binary-300.png < answers.txt". It will take a while to run as there is a one second delay between each answer (To make brute forcing the solutions, less worth it). 	After the program finishes executing you will see " Congratulations, Have a Flag:
  Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook?Ook!Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook?Ook.Ook?Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook?Ook!Ook!Ook.Ook?Ook!Ook!Ook!Ook!Ook!Ook!Ook?Ook.Ook?Ook!Ook.Ook?Ook!Ook!Ook!Ook.Ook!Ook!Ook!Ook!Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook?Ook!Ook!Ook.Ook?Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook?Ook.Ook?Ook!Ook.Ook?Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook?Ook!Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook?Ook.Ook?Ook!Ook.Ook?Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook?Ook!Ook!Ook.Ook?Ook!Ook!Ook!Ook!Ook!Ook!Ook?Ook.Ook?Ook!Ook.Ook?Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook?Ook!Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook?Ook.Ook?Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook.Ook?Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook?Ook!Ook!Ook.Ook?Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook!Ook?Ook.Ook?Ook!Ook.Ook?Ook!Ook!Ook!Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook.Ook!Ook.Ook!Ook!Ook!Ook!Ook!Ook.Ook!Ook!Ook!Ook!Ook!Ook.Ook?Ook." 
      The string of repetitive Ooks is Ook code. If you copy the whole program, starting with 'Ook.' and ending with 'Ook.' into the interpreter you should get the flag as an output. (MCA-4D6C2753)  
 Second Solution 
	Same as the first solution you need to add npiet to the path and move answers2.txt into the same folder as Binary-300.png
	Run the command "npiet -tpic Binary-300.png < answers2.txt" 
	Go get lunch, this will take 3-5 minutes
	When it finishes you will have npiet-trace.png file. When you look at it you will notice that one of the long vertical sections is the only one that lacks a trace. (Usually second from the right) 
	You have to then open Binary300.png in a picture editor that allows the changing of pixels. 
	Edit the Binary 300.png so that it looks like the Solution.png that is in the Solution's folder. 
	Run the "npiet Binary-300.png < answers2.txt" command again, (This will be much faster without the trace. 
	Run the Ook interpreter and you will receive the flag. 

Building it. 
	Building this challenge is a two step process (1 if you are running linux). 

 	For windows you run
	perl moonCcompiler.pl < Binary-400.txt | perl moonshadow.pl > temp.pnm on cygwin and
	pnmtopng temp.pnm >Binary-300.png

	On Linux Run 
	perl moonCcompiler.pl < Binary-400.txt | perl moonshadow.pl | pnmtopng >Binary-300.png


Good luck and happy coding
	  
