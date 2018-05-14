# recipeproject
Recipe Project for BN00100436 for BN509

Project Case Study: Recipe Manager 
Summary: Online System to organise and share recipes


-------
Use cases
role 'public' (no login required):
-------
- can see most recently added public recipes
	Recipes =  text title + text summary + step sequence + ingredients
	+ username of author
	+ list of any comments

	
-------
Use cases
role 'user'
-------

- can view / search recipes in collections
	+/- own collections
	+/- shared collections from other users
	+/- all public recipes


	
- can CRUD personal tags

- can CRUD own recipes
	- can share a recipe with other users
	- can change a recipe from private (default) to public 
		NOTE - cannot change back once public
		once public recipe remains in DB even if user is deleted 
						
	- Recipe = 
		- title
		- summary
		- tags
		- list of ingredients
		- sequence of steps

- can CRUD own collections
	- can share a collection with other users

- up/down vote list of proposed new tags (registered users votes count as 5 votes)

- delete user account

- can add a COMMENT to a recipe


-------
Use cases
role 'admin'
-------
- can CRUD user and admin accounts

-------
EXTRA MARKS
add some or all of these features if going for a high grade
-------

- can upload photo for recipe / for a step of a recipe

- can associate 'tags' with a reciple
	- can see list of tags
	- can propose new candidate tag
	- can see list of proposed new tags
	- up/down vote list of proposed new tags (anonymous users votes count as 1 vote)
	- 'admin'user can accept / reject a proposed tag

- can search recipes by:
	- free text content search for one or two keywords
	- date range (created / last edit)
	- matching one or more tags



HDip Web Software Engineering - Project

You are to develop, test and defend a data-driven PHP website, to illustrate the topics of the module. See the attached diagram specifying the scope of the project, and criteria for different grades.

You submit the project via GitHub repo URL & your published working website URL
	- the Github code URL must be submitted before the Easter break
	
regards,

.. matt ..

NOTE: Sources and plagiarism
This project is an individual project. All work submitted should be your own, except for any images you use, and any HTML/CSS/JS templates. You should document all image and client-side code sources in file /public/sources.txt

All code and text content should be your own original work, with the following exceptions:
- you may use and modify any example code from the lectures/labs/evote-dvd case study without any need to reference such sources. 
- you may (and in fact are encouraged to) use full PHP components installed using Composer. Your composer.json file and vendor folder lists all project dependencies for third-party components, so there is no need to acknowledge any such components any further.

You may NOT use other PHP code inserted into your own classes or scripts - i.e. your PHP code in index.php/setups and all your OO classes must all be your own code. 

While you may get IDEAS for code to solve particular problems from other sources, you must WRITE all lines of code yourself and full understand every line of code in your classes and index.php files. Remember by submitting this project you are declaring that it is all your own individual work unless explicitly and unambiguously acknowledged by you.

There is no need to cite any code:
- from my examples
- from the Symfony and Twig websites
- for any components installed via Composer (since they are cited for you in composer.json)