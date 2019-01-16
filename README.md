# Text-Editor-Project-4


Project 4 COSC 600, Towson University

  Write a program in Java that simulates a simple line editor which supports the following operations:

 $insert
Each subsequent line, up to the next line editor command, will be inserted in the text. If there is a designated current line, each line is inserted before that current line. Otherwise each line is inserted at the end of the text

 $delete m n
Each line in text between lines m and n inclusively will be deleted

 $print m n
	Display the lines m and n inclusively along with their line
     numbers. If the parameters m and n are missing, print the
     entire text

 $line m
	Line m becomes the current line. The program should display up to 3 lines of text along with their line numbers before
     and after the current line depending on whether there is
     enough text in the linked list
 
$search string	
	Search for the string in the text. If found, display the line
     that contains the first occurrence of the string

 $done
	Terminates the execution


Remarks:
. Check for incorrect commands and their parameters and  
  display appropriate messages. For example, if there is no
  the 10th line  in the text and the user types line 10, an
  error message should be displayed
	. Use a linked list to store all text provided by the user
	. All commands of this simplified line editor begin with a $
       symbol
	. If the syntax of a command is incorrect, display an error
       message and let the user try again
	. Having received the command insert, if the first letter of
       the next line is not a $ symbol, treat it as a line of
       text, and store it in a node of the linked list
	. Use StringTokenizer to process a line of text word by 
       word if needed.
     . Always display a message "Please enter a command or a line
       of text" after a command or a line of text is received
     . Always indicate the current line in a displayed text. The
       default current line is the first line, and the first line
       is numbered as line 1.
	. You cannot use the built-in list package
	. Submit your program along with the output file that shows your program can do the following

 Use the following test data to test your program
	$insert
		Golf is indeed the fastest-growing game 
		on an international level.
		A life long game for 
		every golf addict
		In the United States alone there are
		over twenty-five millions golfers,
		playing over 15,000 courses. 
		Once considered the game of the wealthy,
		golf is changing its image. 
		Exclusive clubs are 
		no longer the mode of the day, 
		as architects are building
		courses for the public.
	$delete 3,4
	$print
	$delete 3,2 (wrong)
	$line 3
	insert      (wrong)
	$search Woods
	$line 1
	$insert
		Tiger Woods is a famous golfer
		as well as a wealthy person
	$search Tiger
	Can I input a line of text here? (wrong)
	$print 2,5
	$line 8
	$insert
		When you are out on the golf course,
		it is a different world. The air is
		clear, and the world is a calmer place
		on the golf course, no matter how frustrated
		one gets.
	$print 100  (wrong)
	$display   (wrong)
	$print
	$done








