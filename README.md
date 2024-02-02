In this note, I will create a Dice rolling application that rolls two dice and displays a random number between 1 and 6. As we click the button both dices shake and generate a new number that shows on the upper face of the dice (in dotted form as a standard dice). The numbers shown on the upper face generates randomly each time we roll the dice.

There are two components Die and RollDice. The Die component is responsible to show one individual Dice. It is a stateless component. It uses the font-awesome library to show the standard dots on the upper face of the dice. RollDice component contains all the logic to generate random numbers to show on the upper face of the dice, roll each dice upon click on the roll button. There are two states involved in the RollDice component named ‘die1’ and ‘die2’. Each one has initialized with the value one i.e. each die shows one(one dot) when the application first starts. 

Lets have a quick look at how the final application develpoment will take place- 

Steps to create the Application:

Step 1: Create the application using the following command:
npx create-react-app dice-roll

Step 2: Navigate to the project folder
cd dice-roll

Step 3: Install the required modules.
npm i @fortawesome/fontawesome-svg-core
npm i @fortawesome/free-solid-svg-icons
npm i @fortawesome/react-fontawesome

Step 4: Create a new directory called components
mkdir components

Write the following code in the respective files
App.js component  renders a single RollDice component only.
RollDice.js: It contains all the behind logic. The setting event handler updates all the states according to the user’s interaction render Die component. This file has to be created by you.
RollDice.css: Styling RollDice component contents
Die.js: Responsible to show single-die component only with the correct dotted number face as communicated by the parent RollDice component. This file has to be created by you.
Die.css: Styling each die component and setting animation effects to it.
