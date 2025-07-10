# AWSLexShowcase
Screen shots of a AWS Lex Bot 

## The Flutter Lex UI sends messages to the custom Lex backend which uses the Lex SDK.

The custom LEX RESTful interface sends back responses for the UI.

This screen shot of the FindMyOrder, which calls a Lambda function and returns back a list of records (max 5).
![image](https://github.com/user-attachments/assets/38cd5d15-ae31-4481-b79d-9779044bdc75)


This flutter UI connects to a backend that is the intermediary to the LEX bot defined in AWS Lex
(The intermediary is a springboot RESTful service that is protected with an access token controlled by AWS Cognito -- that is a different story)

![image](https://github.com/user-attachments/assets/a7847df8-6378-4155-babe-224c661bec34)

There are two intents that were written: OrderPizza and FindMyOrder

And here is the slot views of the OrderPizza

![image](https://github.com/user-attachments/assets/52c33bc1-ff89-4385-bd73-d04ddb5645a8)

At the end of the OrderPizza conversation, a AWS Lambda function is used to create an order and send an order email to the registered user.


