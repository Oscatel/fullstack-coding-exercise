## Fullstack Coding Exercise 
### Task   
Create a web application to analyse an SMS message.  The application should     
accept a telephone number and message string submitted by a user and send the data     
to a backend for processing.  The application should then display the following     
information    
    
- Country, Operator and Prefix of the telephone number 
- Message with any urls highlighted and clickable   

A sample dataset of country and operators prefixes is [supplied](./sampledata.json) for Chile, all numbers start with `56`

When matching a number to the prefix the application should select the record with the longest matching prefix from the supplied sample data set, for example

Given a phone number `562198012345`  and a set of prefixes

    {"prefix": 56, "operator": "", "country_code": 56, "country_name": "Chile"},  
    {"prefix": 562, "operator": "", "country_code": 56, "country_name": "Chile"},
    {"prefix": 5621, "operator": "", "country_code": 56, "country_name": "Chile"},
    {"prefix": 562198, "operator": "Chiletel", "country_code": 56, "country_name": "Chile"}

The application should select the record with prefix `562198`
    
### User story 
 - As a user I can **enter a number and message into the application**
 - I can then **see the country, operator and prefix** of the number    
 - I can **click a link** in the message to open the site 
  
### Technical Requirements  
- We'd like you to use [React](https://facebook.github.io/react/) but add whatever ui framework you feel comfortable with 
- Typescript is fine but not required  
- Use any libraries you feel you need 
- The backend should provide a REST endpoint to analyse messages  
- Provide tests  
- Authentication is out of scope of this exercise  
- Write a docker-compose.yml to run the application  
  
### Notes  
Take as little or as much time on this as you feel you need. 
Your time is valuable, so we wouldn't expect you to take more than 2-3 hours on this.  
We're interested in your approach, and ideas as much as we are a working app, 
so if something is not perfect don't worry, just tell us how you would improve it given more time.
  
### Submission  
Please commit your application to a github repository and share with user `d1rtym0nk3y`
