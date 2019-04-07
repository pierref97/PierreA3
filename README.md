# PierreA3

<h1>Pierre Frigon-Assignment 3</h1>
<h1>Project name: AutoBot</h1>

<h2>About the project</h2>
Our project is called Autobot and is essentially an AI that assists a user in picking a vehicle and/or bicycle. This is done by asking the user a series of questions which helps Autobot predict what the user will prefer. Autobot is mainly for users who may have limited knowledge of what type of vehicle they are interested in.

<h2>Navigation for software</h2>
We organized all code in one class (VehicleList) for simplicity and ease of access. VehicleList initiates a database and adds all vehicles available. 
<h2>Code organization</h2>
In VehicleList.py the codes are organized into 4 parts sepearted by comments.
1. Database of cars
2. Text input for text matching check
3. FUnction for text finding 
4. methods for compiling 

<h2>Added features by Pierre</h2>
- A window based GUI, chosen because the closing and opening of a new window replicates the pauses the initial bot incorporated to make it feel more organic.  Also, I find it more interactive and more visually appealing.
  
 - Added bike data so that the user receives an option to choose or request a bike.  It is good for users who wants eco-friendly options or cheaper transportations options.
 
Conversation snippet:  Here is a/an bike. 
                       It is a 2019 Spark Spark, it seats 1 
                       and gets 0 miles to the gallon. 
                       You can walk away with this bike for $1600
 
 - Added a list of 5 different outputs the chatbot will give if it does not recognize an input, which is enables users to understand they did something wrong and adds more interaction and transparency to the chat process
 
 Conversation snippet: What are some important aspects you want in your vehicle? Currently we support the following features: 
 - Fuel efficiency - Seating - Price - Type of Vehicle - Brand
 
 Input: No
 
 Output: I think you have the wrong chatbot
 
  - Using the pre-established Porter Stemmer algorithm in certain places, users can type words in different forms and the chatbot will still recognize it inside the database of possible inputs.
  
   Conversation snippet: What are some important aspects you want in your vehicle? Currently we support the following features: 
 - Fuel efficiency - Seating - Price - Type of Vehicle - Brand
 
 Input: Fueling

Output: What is the worst fuel efficency you would be okay with? 
 
 - Synonym recognition was added using wordnet on the "How are you" question to allow more flexibility for possible user input that the chatbot can respond to
 
  Conversation snippet: How are you today?
  
  Input: Well     (Well is not on the list of possible inputs for the bot, but is a synonym for good)
  
  Output: :).      (One of the possible responses for good)
 

 
