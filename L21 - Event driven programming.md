![[Screenshot 2024-10-23 at 12.54.50.png]]![[Screenshot 2024-10-23 at 12.54.58.png]]![[Screenshot 2024-10-23 at 12.58.20.png]]
# Notes on event-driven programming
- Real world examples: GUIs, web dev (JavaScript), embedded systems.
- Event-driven programming abstraction is often provided by a development framework: e.g. JavaFX (GUI development framework), Web Development Frameworks.
- The flow of the program is based on the state of the program. 
- When events occur, the event is fired, and the listeners implement an 'event handler' method which decides what to do upon this event occurring. So therefore, the events determine the logic/flow of the program

# Example with JavaFX (a GUI dev framework)
![[Screenshot 2024-10-23 at 13.18.40.png]]
![[Screenshot 2024-10-23 at 15.03.48.png]]
![[Screenshot 2024-10-23 at 15.03.57.png]]![[Screenshot 2024-10-23 at 15.04.04.png]]
![[Screenshot 2024-10-23 at 15.04.15.png]]
NOTE: added line 11
# Advantages of event driven programming
- Better **encapsulation** by hiding behavior in classes
- Avoid having to explicitly send information about the input; instead it is automatically passed as part of the callback.
- Easily add/remove behavior to classes
- Easily add/remove behavior to responses
# Observer pattern
![[Screenshot 2024-10-23 at 15.36.57.png]]
# Software development frameworks
![[Screenshot 2024-10-23 at 15.38.36.png]]
![[Screenshot 2024-10-23 at 15.38.50.png]]
