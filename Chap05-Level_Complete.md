# Level Complete

Oh what a great it was after completing a level in Mario!!! 😎🤩
    <br>

![level_complete](https://media.giphy.com/media/dw4sZ2h4aXASKAEXY8/giphy.gif)

Ever wondered what happens in the background that concludes that the level has been completed.

Let's discuss how to conclude whether a level has been completed or not. Basically, there are 2 conditions when a level is marked completed:
    1. When the player has reached the end of the level, a trigger is fired to let the player know that the level has been completed, and then the player is redirected to the next level. 
        a. We are able to achieve this through detection of collision and trigger used to detect collision.
        b. Triggers allow the player to pass through the game object. Triggers are mainly used for tutorials and power-ups.      
        
        
https://user-images.githubusercontent.com/44625252/152813070-c0a2ae26-9b93-4bbd-bb36-a67a5733532a.mp4

![door_coll](https://user-images.githubusercontent.com/44625252/152813112-1d8d0120-c7e7-4feb-9012-363382dd2398.png)

![Dorr_collision](https://user-images.githubusercontent.com/54135921/153474069-658a6968-f666-45cf-972e-41e58eae6952.gif)

In the above video, a collider has been added to the door and the Is Trigger component of the collider has been checked(set to true). So now the door allows the player to pass through it and acts as a Trigger which when comes in contact with the player performs a certain operation i.e. indicates the player that the level is complete and then proceeds to move on to the next level.

    2. When the player has collected the necessary collectables to complete the level is also when we can conclude whether a level is completed or not.
       We do this by keeping a track of the collectables collected by the player after the player has collected one.
       
       
https://user-images.githubusercontent.com/44625252/152813394-e61032e6-c46e-4bfc-bb8a-e4cbbdd75f2a.mp4

In the above sample video, we keep a track of the number of collectables we need in order for the level to get complete. Once we have collected all the stuff we can see a level complete screen pops up at the end of the video 😎
