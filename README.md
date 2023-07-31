Hand Gesture-Controlled Presentation

Welcome to the Hand Gesture-Controlled Presentation repository! This project enables you to control your presentations with hand gestures using computer vision techniques. 
The code uses Python and OpenCV for hand tracking and gesture recognition, making it a fun and interactive way to navigate through your slides.

KEY FEATURES:
Control presentation slides using hand gestures: Navigate forward and backwards using simple hand movements, making it easy to focus on your content without distractions.
Annotate slides in real-time: Draw on the slides during the presentation to emphasize key points and engage your audience.

ABOUT THE PROJECT:

 By using hand gestures as input, the project eliminates the need for traditional input devices such as a mouse or keyboard, providing a more natural and intuitive way to control the presentation. This can be particularly useful in scenarios where a presenter needs to have hands-free control or when using traditional input devices is not practical or accessible.
Overall, the project enhances the user experience by providing a hands-on and interactive approach to navigating and interacting with presentation slides.

VIDEO DEMO: https://www.youtube.com/watch?v=0K8Cpo_7Nks&t=238s

HOW TO USE: 

Here's an explanation of each gesture implemented in the code:

Move to the previous Slide: This gesture is detected when the hand is above the gesture threshold and the index finger is extended while the other fingers are closed. It allows you to navigate to the previous slide in the presentation. The code checks if the fingers are [1, 0, 0, 0, 0], indicating that only the thumb is extended.

Move to Next Slide: This gesture is detected when the hand is above the gesture threshold and the little finger is extended while the other fingers are closed. It allows you to navigate to the next slide in the presentation. The code checks if the fingers are [0, 0, 0, 0, 1], indicating that only the little finger is extended.

Mouse Pointer Gesture: This gesture is detected when the hand is above the gesture threshold and the index and middle fingers are extended while the other fingers are closed. It enables a pointer, where you point anywhere on the slide using the pointer(a red circle). The code checks if the fingers are [0, 1, 1, 0, 0], indicating that the index and middle fingers are extended

Draw Annotation Gesture: This gesture is detected when the hand is above the gesture threshold and the index finger is extended while the other fingers are closed. It enables us to annotate on the slide. The code checks if the fingers are [0, 1, 0, 0, 0], indicating that the index finger is extended.

Delete Annotation Gesture: This gesture is detected when the hand is above the gesture threshold and the index, middle and ring fingers are extended while the other fingers are closed. It enables us to delete the annotation. The code checks if the fingers are [1, 1, 1, 0, 0], indicating that the index and middle fingers are extended

REQUIREMENTS:
Python 3.x

OpenCV (cv zone and numpy dependencies)

Webcam or external camera

GETTING STARTED:

Clone the repository to your local machine.

Install the required dependencies using pip install -r requirements.txt.

Ensure you have a working webcam or external camera connected to your computer.

Run the script hand_gesture_control.py and present your slides using hand gestures.

