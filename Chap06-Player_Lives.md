# Player Lives

- To create a Life system we need to do things, first one is the Sprite that we will be displayed on the screen for the user, the second is a controller which decreases a life whenever the player collides with an enemy or increase a life when the user collects a power-up that restores a lost life.
- The very first step to creating a Life system is to start by creating a sprite that will be displayed on the screen for the player that will be indicating how many lives are remaining for the player.

![Lives](https://user-images.githubusercontent.com/44625252/152813950-c660cb5d-e4ec-4575-b74a-da04c3aa6438.png)

![Lives_hie](https://user-images.githubusercontent.com/44625252/152813968-8cc27b4d-2e29-4a27-823f-483d59d64740.png)

- The next step is to add a method that will decrease the life by one whenever our player collides with the enemy. We can start by detecting the collision in our Enemy Controller and if the collision is with the player we decrease the life by one.
- To decrease the life in real time we will be assigning these sprites to our game objects that we have created in our script and we will simply set its visibility to false whenever the player collides with an enemy. by doing so it will appear as if the lives are being decreased but in reality, we are simply changing the values of visibility of the sprite.

![Lives_scrp](https://user-images.githubusercontent.com/44625252/152814056-dd39a099-f256-4109-b10f-1516fb30c8fc.png)

- Now, you might be thinking there might be a time when the player will run out of lives what happens in this scenario?? well basically this is where we make the game over for the player.
- Once the whole implementation is done correctly this is what the final output must look like. 🤩

https://user-images.githubusercontent.com/44625252/152814148-b1c2369a-f78e-4afb-b0c8-4f79f18625ad.mp4

---
<aside>

> 💡 🚀 **[Join Discord Server](https://discord.gg/J5zDscnzms) → Get your doubts solved by experts instantly**
</aside>

![discord_png](https://user-images.githubusercontent.com/44625252/152805317-45a22cd7-fbf5-49cc-a13d-01282d498b03.png)

---
