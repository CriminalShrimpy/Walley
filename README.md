OPEN COMMAND PROMPT AND CHANGE THE DIRECTORY TO THE PYTHON
EVIRONMENT THAT YOUR EDITOR IS USING (THE VERSION MUST BE 3.11.2)
THEN TYPE IN THE FOLLOWING LINES OF CODE

FIRST UPGRADE THE PIP WITH
python -m pip install --upgrade pip

#CHECK IF YOUR PIP VERSION IS UP TO DATE (SHOULD CURRENTLY BE 23.0.1)
pip --version

THEN INSTALL THE FOLLOWING
pip install nltk
pip install tflearn
pip install tensorflow




#HERE IS A BRIEF DESCRIPTION OF HOW THE BOT WORKS

This is a program written in Python that uses natural 
language processing (NLP) methods and a neural network 
to construct a very basic conversational bot. The following 
libraries are used in the program: nltk, numpy, tflearn, tensorflow, 
json, pickle, random, tkinter, and PIL.

The chatbot is trained using a collection of pre-defined patterns 
and replies provided in the actions.json JSON file. These patterns 
are tokenized using the nltk package, and the tokens are stemmed using 
the LancasterStemmer class. Following that, the stemmed tokens are utilized 
to form a "bag of words" for each pattern.

The application then builds a neural network with the help of the tflearn 
and tensorflow libraries. The neural network is made up of three hidden 
layers, each with ten neurons, and an output layer with the same number 
of neurons as the number of potential replies. The neural network is 
trained with 500 epochs and an 8-batch size using the fit function.

Following training, the application generates a graphical user interface 
(GUI) window using the tkinter library. The GUI window includes a chat window, 
a user input area, and a send button. When a user writes a message into the 
input field and hits the send button, the application predicts the neural 
network's most likely answer and displays it in the chat window.

The algorithm tokenizes the user input, stems the tokens, and generates a 
bag of words to anticipate the answer. The software then uses the predict 
function to input the bag of words to the neural network. The most likely 
response is picked, and a random response from the selected response list is 
presented in the chat window.
