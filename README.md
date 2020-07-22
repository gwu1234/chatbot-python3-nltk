it is self-education practice to build a toy chatbot from nltk.

For a good explanation, please refer to https://medium.com/analytics-vidhya/building-a-simple-chatbot-in-python-using-nltk-7c8c8215ac6e


1) create python3 env

pip3 install pipenv

pipenv shell

pipenv install nltk numpy  sklearn

2) download nltk_data 

open pythons shell (python3)

import nltk

import ssl

try:

    _create_unverified_https_context = ssl._create_unverified_context

except AttributeError:

    pass

else:

    ssl._create_default_https_context = _create_unverified_https_context

nltk.download()

select all packages

3) In this practice, we use chatbot.txt as our corpus.

4) In this practice, response is based on the similarity between words entered by the user 

and the words in the corpus. 

5) test chatbot

python3 chatbot.py 

testing utterances: 

hi

hello

what is chatbot

what is guoping wu

what is nuance

bye