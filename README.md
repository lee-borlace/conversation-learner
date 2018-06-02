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




