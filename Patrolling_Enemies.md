# 9. Patrolling Enemies

Basically, there are 2 ways of making enemies patrol in a specific area.

  1. Using waypoints: we can set waypoints and make the game object travel within those waypoints. Below is a piece of code for further reference.
  
  ![Enemy_Patrol_wp](https://user-images.githubusercontent.com/44625252/152816830-39abcdbb-3327-40a7-ac92-517e3f578b6d.png)
  
  In the above code, we are calculating the distance between the waypoint and our enemy game object. By doing so once we get the distance which is less than 0.01f we are changing the waypoint to the other one that is set by the user in the Unity inspector and we are also flipping/rotating our game object so that it is facing towards the other waypoint. So, it goes on like a loop and the game object keeps on moving within the waypoints. 😎
  
  2. Using Raycasts : A Raycast is like a laser beam fired from a point that we call as “Origin” along a particular direction to detect if our game object is still in collision with the other game object and if it is not in collision we perform certain operations. The big advantage is that every object which makes contact with the laser beam can be reported!

  ![Patrolling_enemy_raycast](https://user-images.githubusercontent.com/44625252/152816986-881e7d93-a619-4dea-9bda-7aad1e4f4c90.png)

  In the above code, RaycastHit2D returns information about an object detected by a raycast in 2D physics. The RaycastHit2D class is used by Physics2D.Raycast and other functions to return information about the objects detected within the range fired by raycasts. 👾

---
<aside>

> 💡 🚀 **[Join Discord Server](https://discord.gg/J5zDscnzms) → Get your doubts solved by experts instantly**
</aside>

![discord_png](https://user-images.githubusercontent.com/44625252/152805317-45a22cd7-fbf5-49cc-a13d-01282d498b03.png)

---
