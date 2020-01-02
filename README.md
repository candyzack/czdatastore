Author: Deep Baldha

## File Structure

"source_code.py" :  is the source code of the Flask app. 
		    It handles API calls and saving data of Python Dictionary in Persistence File.
		    
"cli.py"         :  is the python source code for CLI.

## Deployment

Flask App is deployed on Heroku.
URL is https://czdatastore.herokuapp.com <br>
APIs example are as fellow:

1) https://czdatastore.herokuapp.com/set/foo:104
2) https://czdatastore.herokuapp.com/get/foo
3) https://czdatastore.herokuapp.com/reset/iron

Above API calls returns JSON datafiles.
Password for reset is "iron".

## How to Use CLI.py

In terminal/cmd:

1) python cli.py set <KEY> <VALUE>
	
	example: cli set foo 104

	This command is used to store value VALUE under key KEY in datastore
	Also gives confirmation on successful storage

2) python cli.py get <KEY>
	
	example: cli get foo
	
	This command is used to get value of key KEY from the datastore
	Return "null" is not value

3) python cli.py reset <PassWord>
	
	example: cli reset iron
	
	This command is used to reset the database and delete all the key:value pairs from datastore

