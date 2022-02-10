# UI Basics

What is a UI???
    
UI or User Interface is something which allows the User to interact with or to be specific with game development it is something that allows a Player to interact with. Unity UI is a UI toolkit for developing user interfaces for games and applications. It is a Game Object-based UI system that uses Components and the Game View to arrange, position, and style user interfaces.

![user interface](https://media.giphy.com/media/l1J9qemh1La8b0Rag/giphy.gif)
    
![UI_1](https://user-images.githubusercontent.com/44625252/152817533-adecc32e-c6b2-4aa8-8435-c7ed3eae803f.png)
    
![UI_2_2](https://user-images.githubusercontent.com/44625252/152817591-8e1e386a-5fcb-46e9-8073-87aeb61644b7.png)
    
- Above snapshots show images of Main Menus of games. These main menus are the best examples of UI used in games. Obviously any game will have a menu. When we press on the buttons say single player or exit button then it will either start the game or exit the game by the functionality that has been assigned to the button itself.
- Some of the main components of UI are:
    - Canvas
    - Buttons
    - Texts
    - Panel
    - Slider

1. Canvas
    - You might have heard that we generally use Canvas whenever we are trying to paint something. It is mostly used by professional artists to show their art on the canvas.
    - Basically, canvas is a sheet where you can draw or wrt game development canvas is a component where you can draw your UI.
    - Whenever you add a UI component Canvas will also be added along with it.
    - To insert a Canvas, right click in the Scene Hierarchy and go to Create → UI → Canvas.

![UI_2](https://user-images.githubusercontent.com/44625252/152817805-3aec02e3-d6d6-41da-8384-435943c09955.png)

2. Buttons
    - Anything when clicked and performs an action after it has been clicked is called a button. In real life we have a switch/button to turn the light on/off in the same we have UI buttons for certain operations.
    - In game development we can consider a mouse button which when clicked during a game might fire a weapon or do any other operation assigned to it depending upon the game.
    - To insert a button, right click in the Scene Hierarchy and go to Create → UI → Button. If you do not have an existing Canvas and an Event System, Unity will automatically create one for you, and place the button inside the Canvas

![UI_buttons](https://user-images.githubusercontent.com/44625252/152818026-60137f58-37f7-4b21-b1f0-5c8bc268eded.png)

3. Texts
    - Every game has a name which is displayed in the UI and for displaying those names we use UI Texts.
    - Texts are non – interactable they’re used for displaying some information. For eg: it can be used to display instructions or it can be used to display a player’s current score in the game.
    - To insert a Text, right click in the Scene Hierarchy and go to Create → UI → Text.

![UI_text](https://user-images.githubusercontent.com/44625252/152818146-959fcfde-45da-4ac3-b69a-8b78cbd7ef8f.png)

4. Panel
    - Panel is a UI component that acts as a container in Unity.
    - It helps us in grouping together different UI elements.
    - Panel defines an area that will by default stretch to fit its parent RectTransform dimensions.
    - To insert a Panel, right click in the Scene Hierarchy and go to Create → UI → Panel.

![UI_panel](https://user-images.githubusercontent.com/44625252/152818210-f7965327-8272-4b0b-bec0-0801792e36c7.png)

    
5. Slider
    - The Slider UI element is commonly used where a certain value should be set between a minimum and maximum value pair.
    - One of the most common usages of this is for audio volume, screen brightness, or for doing zoom.
    - To create a slider UI, right-click on the scene hierarchy and select Game Object -> UI -> Slider. A new slider element will display on your scene.

![UI_Slider](https://user-images.githubusercontent.com/44625252/152818314-a9fdc480-2f46-449c-8386-ed9655019f0c.png)

---

