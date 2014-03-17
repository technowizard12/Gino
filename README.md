#Gino
##Gino Is a Natural Organizer

Gino is a task prioritization tool for those of us who are completely incompetent when it comes to such things, such as the author. Adhering to the "Eisenhower Grid System", Gino prioritizes tasks based off of user-reported importance/urgency (with the added twist of organizing based off of due date, which is not necessarily a component of the original system). 

Gino is also devilishly suave. And even more devilishly minimalist.

###General Principle

This program is the core of Gino. It does nothing but the organizational meat. Gino may interface with GUIs or web interfaces, but this project contains the essence of Gino, whose functions are as follows.

* Process input
  * Item Title
  * Urgent yes/no
  * Important yes/no
  * Due Date
* Compile Prioritized List
  * Using one of two formats
    * Daybreak DB
    * Text File
* Generate Some Sort of Witty Quip
  * What's an assistant without snark?

###Dependencies

* Chronic: https://github.com/mojombo/chronic
* Daybreak: http://propublica.github.io/daybreak/
* Good humor

###Methods and Such

_NOTE: while this information may be found in the class documentaiton proper, it's repeated here for clarity's sake, since the README is the first bastion of documentation_

####To add a new task:
	
	`Gino.input(title urgent, important, due date)`

#####Arguments:

  title - A string; the title for the task
	urgent - A boolean; true for urgent, false for not urgent
	important - A boolean; true for important, false for not important
	due date - A string, representing the date due. To be parsed using Chronic.

####To compile a prioritized list

  `Gino.output(format, location)`

#####Arguments:
	
  format - A string indicating format to output to. "text" for plaintext file. Defaults to Daybreak DB.
  location - Locatino to write the file to

####To generate a witty quip

  `Gino.quip`

  Which will cause Gino to put a witty quip.

###License

This software is released under the WTFPL version 2 by Simon D. Orr. License follows.
>
>            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE 
>   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION 
>
>  0. You just DO WHAT THE FUCK YOU WANT TO.