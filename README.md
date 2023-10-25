# miscAI
Some notes and code from playing around with misc. AI, mostly GPT-4 and the openai APIs so far.

Scrips assume API keys are in the keyring.
Use something like this to set it:

import keyring
# Set the API key then delete this so it's not laying around
keyring.set_password("system","openai_api_key", "delete this line after running because it would be a API key")



Then in the code you'll see something like:
# Retrieve API key from the system keyring
openai.api_key = keyring.get_password("system", "openai_api_key")

Deps so far:
pip install openai keyring
