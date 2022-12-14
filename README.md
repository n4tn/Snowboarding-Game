# **Snowboarder!**
![Image](./ScreenCaps/Snowboarding.PNG)

- [Aim of the Game](#Aim-of-the-Game)
- [Controls](#Controls)
- [Build Process](#Build-Process)
- [Future Improvements](#Potential-Improvements) 

## Aim of the Game
 Get the snowboarder from the start of the level to the end of the level without crashing or falling off the map.

## Controls
 - Left and Right Arrow keys control the rotation for back or front flips!
 - Up Arrow key allows for a small boost!

## Build Process 
 - Used Sprite Shapes to design the base for our level
 - Used edge colliders to attach to the base of our level
 - Used Cinemachine to make a follow camera that follows the player
 - Used a surface effector to create a "Conveyor belt so our snowboarder constantly is accelerating forward"
 - Added Torque to our snowboarder so they can spin and do either front or back flips in the air
 - Added two triggers:
   1. Finish Line to complete the level
   2. A crash trigger on the snowboarders head to  restart the level
 - Imported UnityEngine.SceneManagement and used the SceneManager class method LoadScene to restart the surrent level if the player hits either of the two triggers above
 - Used Invoke to create a pause before reloading the level if a trigger is hit (uses string param. of a method name - be careful)
 - Added a Particle system that consists of an emitter and particles and use modules to control the behaviour. Added one for the finish line and a crash trigger
 - Used FindObjectOfType to access the surface effector from a different game object in order to speed up and slow down our snowboarder
 - Using OnCollisionExit2D to allow snowboarding particle effects when touching the ground and no particle effects when not touching the ground
 - Adding Audio
   - Audio Listener (like a microphone)
   - Audio Source (plays and adjusts volume)
   - Audio Clip (audio data to be played)
 - Added an audio clip for both triggers
 - Disabled movement when head collision with ground occurs (making a method public)
 - Prevented the head collision sound playing more than once by using a bool and conditional AND statement 
 
 ## Potential Improvements 
  - Add a time limit
  - Add a style points system where if the user does backflips or frontflips their score increases
  - Add more levels
  - Make the levels longer
  - Add a UI
 
  Any other suggestions for improvements welcome! :)

### Made with help from Udemy
