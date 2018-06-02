# conversation-learner
## Links
https://docs.microsoft.com/en-us/azure/cognitive-services/labs/conversation-learner/overview
https://github.com/Microsoft/ConversationLearner-Samples
http://localhost:5050/home


## Learnings from getting the sample running
### fetch_ponyfill missing
This was initially missing when running. 

See :

https://github.com/Microsoft/ConversationLearner-Samples/issues/198

https://github.com/Microsoft/ConversationLearner-Samples/pull/197

The first time I ran ```npm install``` it errored out with ```gyp ERR! stack Error: Can't find Python executable``` as described in the readme, so it looks like it didn't install all modules. Running ```npm install``` again seems to have fixed it.

### Training
I had issues selecting an action after labelling a sample input with entities. It would let me choose my API action etc, but then the buttons to backtrack the step or finish training became greyed out. All I could do was abandon the training.

## Learnings about how the bot works
Bot logic is defined in ```app.ts```. Points of interest are ```cl.EntityDetectionCallback()``` (entity processing) and ```cl.AddAPICallback()``` (custom APIs to be called).

If you change the signature of an API method, you need to re-start the bot before the UI will pick up the change.



## Sample bots in this repo
### 


