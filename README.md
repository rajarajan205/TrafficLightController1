[Uploading README.txt…]()
SMART TRAFFIC LIGHT MANAGEMENT SYSTEM
=====================================

Requirements
------------
- JDK 17 or newer recommended (JDK 8+ should work)
- Visual Studio Code
- VS Code Extension Pack for Java (Microsoft)

Project contents
----------------
TrafficLightController.java : Complete Java Swing application

Features
--------
- Two simulated intersections
- Start / Stop / Reset controls
- Editable red, yellow, and green timings (milliseconds)
- Simulated Low / Medium / High vehicle density; high density receives longer green time
- Peak Hour Mode
- Ambulance Priority (forces green at both simulated intersections)
- Night Mode (blinking yellow)
- Swing Timer-based signal sequencing

Important limitation
--------------------
Vehicle density is simulated using the dropdown. The project does not currently connect to a
camera, real traffic sensor, or physical traffic signal. Explain this accurately in an interview.

Run in VS Code
--------------
1. Install a JDK and verify from a new terminal:
     java -version
     javac -version
2. Install the Microsoft "Extension Pack for Java" in VS Code.
3. Extract this ZIP to a folder.
4. In VS Code choose File > Open Folder and select the extracted SmartTrafficLightProject folder.
5. Open TrafficLightController.java.
6. Click Run above the main method, or use Terminal > New Terminal and run:
     javac TrafficLightController.java
     java TrafficLightController
7. Click Start. Try Low / Medium / High then Update Density. Try Peak Hour, Ambulance Priority,
   and Night Mode. Use Reset to return to the initial state.

If VS Code does not show Run:
- Ensure the JDK is installed (not only a JRE).
- Close and reopen VS Code after installing the JDK.
- Open the folder, not just the individual Java file.
- Run the javac/java commands in the terminal as shown above.

Interview explanation
---------------------
"This is a Java Swing desktop simulation of a smart traffic-light controller. The interface is
built with JFrame, JPanel, JLabel, JButton, JTextField, JComboBox and JCheckBox. A Swing Timer
cycles through green, yellow and red phases. Traffic density is simulated as Low, Medium or High;
the application gives a longer green interval to higher density. Separate control modes demonstrate
peak-hour timing, ambulance priority, and blinking yellow night mode. Two intersection panels show
the same control state. In a real deployment, vehicle density would need to come from sensors or
computer vision and the controller would need safety interlocks and hardware integration."
