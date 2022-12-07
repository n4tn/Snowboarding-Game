# Snowboarding_Game
Snowboarding game I made in Unity with the help of Udemy

# Basic Content that makes up the snowboarding game

- Used Sprite Shapes to design the base for our level
- Used edge colliders to attach to the base of our level
- Used Cinemachine to make a follow camera that follows the player
- Used a surface effector to create a "Conveyor belt so our snowboarder constantly is accelerating forward"
- Added Torque to our snowboarder so they can spin and do either front or back flips in the air
- Added two triggers:
  1. Finish Line to complete the level
  2. A crash trigger on the snowboarders head to  restart the level
- Imported UnityEngine.SceneManagement and used the SceneManager class method LoadScene to restart the surrent level if the player hits either of the two triggers above
