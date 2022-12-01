[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-c66648af7eb3fe8bc4f294546bfd86ef473780cde1dea487d3c4ff354943c9ae.svg)](https://classroom.github.com/online_ide?assignment_repo_id=8858470&assignment_repo_type=AssignmentRepo)
# Virtual Pet
 
Authors: [Bilal Suleiman](https://github.com/bsule), [Brent Nicks](https://github.com/brentnicks), [Lauren Gager](https://github.com/MinteaAliens), [Adrian Franco](https://github.com/afranco7645)

# Phase 1
## Project Description
 * We think this project would be interesting because it stands out from common project ideas and has a scalable project scope. Additionally, including minigames should allow for more seemless development since they can be created independent of each other.
 * We will primarily be using C++ for this project.
 * Our project will take user input when playing minigames, choosing which of two pets to take care of, choosing different clothes for that pet, cleaning, and feeding it. The outputs will be the virtual pet made from different ASCII character, minigame interactions, and different options for the user to choose in the UI. 
 * This project will show a virtual pet on the screen that the user can customize. It will have minigames that unlock different items for the pet along with a level up system that reveals something new for the user to enjoy and progress towards. More features include feeding the pet, giving it different clothes, and saving the users progress by creating a file which contains the level of the pet and the different customizations it has unlocked. The pet will also have its own values for status such as hunger or happiness that will increase as the user interacts with the pet. Minigames may include blackjack, rock paper scissors, tic-tac-toe, and connect 4.
 * We strive to imitate old 2000's games/toys such as the Tamagotchi and Neopets to allow young adults our age the chance to relive their virtual pet experience.

# Phase 2
UML: https://lucid.app/lucidchart/6ec63cb4-8ba2-4973-b340-eee9c70e0c05/edit?viewport_loc=-107%2C-104%2C1664%2C831%2C0_0&invitationId=inv_7dd7caaf-efac-4b64-8fa4-2b58c10aefb0

<img width="693" alt="image" src="https://user-images.githubusercontent.com/48264066/204424715-97516e5a-18bc-4233-8e36-edc61cd973b6.png">

## Uml Diagram Description

Our uml diagram outlines a VirtualPet class with many different functions and variables to keep track of the users virtual pet. These include getHunger, getThirst, getExperience, getPetType, and many more all designed to make the user feel connected with their pet. 

The user will be able to use functions such as feed, drink, or rest in order to improve the status of the pet. Through the printXPtoFile function, the user will be able to save their data to a file in order to save their progress. 

Our other class is a Minigames class which has games that include TicTacToe, RockPaperScissors, Blackjack, and Connect 4. The point of these minigames is to be able to level up the pet and unlock new items for it such as accessories that it can wear. 

In TicTacToe and Connect 4, the user will play against the computer and will be prompted to choose a location to place the required input. For RockPaperScissors, the user will choose which object he would like to use and the computer will randomly select one of the three options. Winning the minigames will award xp for the pet and also reward the player with an item for their pet. 

The minigames will have access to the pet's functions like addExperience, printLevelUp, getExperience, printInventory, addToInventory, printXPtoFile, etc. The minigames will inherit from the minigames class because they should be children of the class.

Main will construct the minigame objects when the user calls them and the user will then be able to play the minigames through their functions. The main class of this game is the GameManager which links the inventory and xp features of the pet to minigame xp and item rewards. It is also responsible for broad mechanics such as starting the game and the save/load system.

Game UI: https://docs.google.com/document/d/1W3jxDPH0fONRdmCUfu9zne_PX5xm9ZGd7CwLV0dVn-E/edit#

# Phase 4
 
 ## Screenshots
 ### Main menu
 <img width="327" alt="image" src="https://user-images.githubusercontent.com/48264066/204424358-d60b4f51-a023-465c-a052-5eb062035022.png">
 
### Blackjack
 <img width="612" alt="image" src="https://user-images.githubusercontent.com/48264066/204424170-01d7a57d-a75c-4369-9c7a-d2c6b34e081c.png">
 
### Connect 4
<img width="417" alt="image" src="https://user-images.githubusercontent.com/48264066/204424206-593b0704-30f7-4020-a774-2b60266f53c5.png">

### Feeding pet
<img width="459" alt="image" src="https://user-images.githubusercontent.com/48264066/204424267-b86d4a9d-4d29-468d-8c74-e241b5316ee0.png">

### Checking inventory
<img width="549" alt="image" src="https://user-images.githubusercontent.com/48264066/204424295-f88fded1-edaa-4c51-a546-f9948ccead5e.png">

### Pet screen after playing
![image](https://user-images.githubusercontent.com/48264066/204594295-4a99e1f0-25b8-4ce5-b8bd-371ca76cd00a.png)


### Rock paper scissors
<img width="409" alt="image" src="https://user-images.githubusercontent.com/48264066/204424382-ce325d05-3230-44ed-a24a-5731ae4f90cd.png">

### Tic tac toe
<img width="268" alt="image" src="https://user-images.githubusercontent.com/48264066/204424404-e64e387d-aefb-4eb7-a0ad-6adb735b5f3f.png">

### Tests
<img width="302" alt="image" src="https://user-images.githubusercontent.com/48264066/204621168-d0070921-5c9c-4e0e-a119-1291bbc09c95.png">
<img width="394" alt="image" src="https://user-images.githubusercontent.com/48264066/204621359-f471e972-184a-456d-8604-2eae7d38f763.png">
<img width="374" alt="image" src="https://user-images.githubusercontent.com/48264066/204621449-f8fd38f9-8a39-4a5a-8efe-d9d802fcb730.png">
<img width="389" alt="image" src="https://user-images.githubusercontent.com/48264066/204621563-bc536df4-ce58-4f65-b74c-8eb4bd682960.png">
<img width="394" alt="image" src="https://user-images.githubusercontent.com/48264066/204621638-b1e93746-2fcb-4c63-b320-6e4eea8fc813.png">
<img width="388" alt="image" src="https://user-images.githubusercontent.com/48264066/204621689-4e279d5c-1e79-49e8-ad9c-6b12e39edca7.png">


 ## Installation/Usage
 To install the game click the green dropdown button with the label "<> Code" then "Download ZIP". After that you can unzip the folder and open in an IDE such as VS Code. Another option is to click the same dropdown as mentioned previously then copy the https link and type git clone --recursive <project-clone-url> into your IDE terminal. Next ensure you are in the root directory and run BOTH "cmake ." and "make" inside the terminal to ensure the game builds properly. Finally you can run the game by typing "./bin/gameManager".
 ## Testing
 Our project was tested via the Google Tests submodule. The only files that required testing were ones that involved logic such as the minigames. It is not necessary to test UI files since it is obvious whether or not they are working properly. Additionally, we checked for a mulitude of edge cases and performed hours of QA testing.
 We also used 'new', so we needed to make sure we didn't have any memory leaks. To check this, we used Valgrind.
