# Chat-Who

Chat-Who is an Chat Bot which is build using the concepts of NLP and CNN.

![alt text](http://url/to/img.png)

## Workflow for creating this project:

1. Initally, a JSON file is created which contains a "Tag" that represents the class of the question, its corresponding "Patterns" that can be asked to the chatbot, and "Responses" that contains possible reply for the question.

2. Incorporating NLP Concepts:
NLP concepts like stemming(generating root form of the words), tokenization(splitting the words into units) and bag of words are used for processing the inputs from the user

3. PyTorch model:
After getting the data and performing the NLP functions, a Feed forward Neural Network (CNN) of 3 layers is build which taked in the bag of words, process and a Softmax function is applied to get the prediction with respect to each tag. The highest probability tag is choosen and a random response is given from the mentioned responses in the JSON file.

After training the model, the data is saved which contains details regarding the model. This data file can be imported in any other file and the model can be used

4. Integrating the model in a Web App:
The model that is trained can now be integrated with an Web Application which can be used as an real time chatbot for the Organization.
