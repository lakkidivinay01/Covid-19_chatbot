# Covid-19_chatbot
Covid-19 FAQ Chatbot
Coronavirus is widely spreading and  several new variants are developing and being heard in the news everyday.It is important to wear a mask and maintain social distance .It is very important for a country like India which is vastly populated where the virus can spread easily. People can use this chatbots/FAQs for help during the coronavirus pandemic to overcome the infection and to know the exact information rather than the rumors. It helps in avoiding ambiguity and misconception regarding what to be followed and how the situation outside etc.Since it is powered by Ai and built on cloud , there will be no downtime and can be scaled based  on incoming traffic easily and it is very secure to use the azure cloud platform . With QnA maker we can built the bot easily without much explicit coding.
In this we are azure machine learning and ai , QnA maker cognitive service to implement the required bot.
The bot can be deployed and embedded in an html we page, Here I used google sites for creating and hosting the webpage.



I used free services in azure to make this bot.QnA maker is a easy and simple to use service.

For the knowledge base during the creation of QnA service , i used docs(url) from the internet.

1)First of all i created resource group(chatbot) for the chatbot tresouces to be deployed.

![image](https://user-images.githubusercontent.com/86817867/162633237-b59be056-9070-4c1a-9775-550ed580c51d.png)



2) Then I created QnA maker resouce in the chatbot resouce group named VinayCovidChatBot
![image](https://user-images.githubusercontent.com/86817867/162633368-ae70fee0-0399-48bf-8e1e-4632d998ad7d.png)




3) I created a knowledge base in the QnA maker service and added QnA pairs from the web.
![image](https://user-images.githubusercontent.com/86817867/162633523-d50ab4be-9a04-4f12-bea6-cc37b6ddb33d.png)
We can also add the Question - Answer pair explicitly to react to the questions that people may ask.





4)We have to save and train the bot on the dataset and we need to publish it. We need to publish the Knowledge base into a bot by using the option create bot .
The bot will get created in the resource group.Then in the channels we shoul select web chat and should copy the code that should be embedded into an html page.
We should also save the secret keys.

![image](https://user-images.githubusercontent.com/86817867/162634014-1ca9c59f-b7ef-46f7-aca5-0908c5cefe31.png)


![image](https://user-images.githubusercontent.com/86817867/162634026-2454d996-570e-4019-a500-97f8a8d520d6.png)


5) We have to embed the code into our own html page that is custom designed.


6) To host the html page we will use the azure storage account static web pages.We should create a storage account.
Here it is covidchatbot.

![image](https://user-images.githubusercontent.com/86817867/162634145-26ea2bf7-1013-4d5a-9b0b-d0e0deae6f44.png)


7)Then in the static website,we should enable it first , we should add our index.html file and should notedown the primary endpoint to access it over the internet.
![image](https://user-images.githubusercontent.com/86817867/162634212-7b031d1c-278d-4e8b-97ce-9ea773ae1fcf.png)



8) Here is the demo link-
https://covidchatbot.z10.web.core.windows.net/



9)Atlast you can see the hosted web page like this. We can enter our query in the type message box to enquire about covid-19

![image](https://user-images.githubusercontent.com/86817867/162634316-5188370b-e825-4f91-85b0-c9e76508a56d.png)


Here We used Azure storage account to host website, Azure bot service to create and deploy bot and azure QnA maker service to create bots.
THus we have created the Covid-19 FAQ bot effortlessly with user at free of cost.



















I have uploaded the bot source code zip file in the present repository.
