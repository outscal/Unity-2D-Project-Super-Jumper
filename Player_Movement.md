Player Movement can be achieved in different ways in unity, depending on the specific requirement, few are:
- Changing Transform.position of the player every frame based on input direction, this process is usually best when no Rigidbody is there and the object simply needs to shift every frame, for eg, in the case of a top-down camera game like Snake
- Force - Applies a gradual force on the Object, taking mass into account. This is a literal pushing motion where the bigger the mass of the object, the slower it will speed up
- Impulse - Applies an instant force on the Object, taking mass into account. This pushes the Object using the entire force in a single frame. Again, the bigger the mass of the object, the less effect this will have. Great for recoil or jump functions
- Acceleration - Same as ForceMode.Force except that it doesn't take mass into account. No matter how big the mass of the object, it will accelerate at a constant rate
- VelocityChange - Same as ForceMode.Impulse and again doesn't take mass into account. It will literally add the force to the Object's velocity in a single frame
