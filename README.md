# IMPORTANT
Since the API has been [discontinued](https://t.me/Intellivoid/559), this will no longer work. 

# About
A fun telegram userbot written in python3 using [EzilaAnki](https://github.com/TeamEzila-Ankivector)'s Coffeehouse API.
Written by [this person](https://t.me/TheRealPhoenix)!
## Installation
Open up your terminal and run these commands.

• ```git clone https://github.com/rsktg/Chatbot.git```

• ```cd Chatbot```

• ```pip install -r requirements.txt```

• Now make a copy of ```sample_config.ini``` and rename it to ```config.ini``` and enter your ```api_id``` and ```api_hash```. These can be obtained from [here](https://my.telegram.org).

### Non-Heroku users
Edit ```NAME``` in ```generate_session.py```

• ```python3 generate_session.py```

### Heroku users
• ```python3 string_session.py```

You'll be asked to enter your phone number and 2FA password (if any). Copy and save the string session you get in the end.

### Two possible ways of going forward
You can either use environment variables or edit the config.ini file further.

If you're going to use environment variables, then add a variable named ```ENV``` and set the value to anything you want.
Now you can use environment variables.

Add the following ones as well.

• ```SESSION_NAME```: If you ran ```generate_session.py```, the name of the session you created.

• ```STRING_SESSION```: The string session (Only for Heroku users).

• ```CF_API_KEY```: You can get this API key from [here](https://coffeehouse.intellivoid.net)

• ```DATABASE_URL```: The URL of your SQL database. It should look something like this - ```sqldbtype://username:pw@hostname:port/db_name```.
PostgreSQL is recommended.

• ```NAME```: Your bot will reply to the AI-enabled users everytime this name is said.

However, if you're gonna use ```config.ini```, go ahead and set the values given above with the exception of ```ENV```.

## Running the bot
After setting the required environment variables/editing the ```config.ini``` file, run ```python3 -m chatbot```.

Congrats, your bot should now be up!

## Credits
• [EzilaAnki](https://github.com/TeamEzila-Ankivector) for providing the API used for this project.

• [SLBOTs](https://github.com/slbotofficial11) - the library used for this project.
