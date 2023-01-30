# Traffic-Light-Control-System---A-Model-Based-Software-Design-Approach
In this project, a Traffic Light Control System (TLCS) using Model-Based Software Design approch. The project implements according to Agile Software Development Process, which starts with project planning and lists system requirement in a Requirement Specification Sheet. Then the TLCS system architecture is developed using a software design approach. Later, utilizing Simulink/State Flow Graphs, a Software Design Block diagram is created and put into use. Following that, a test harness is made, and several test cases are checked to see if the project's criteria were being satisfied.

The task is to create a new traffic light control system that manages the lights for pedestrians and autos automatically. The system must respond to push-button requests made by the user. An optical indication must be used to signify the requests. The following exclusive states are possible for automobile lights:

- green
- yellow
- red
- red-yellow

The exclusive states for pedestrian lights are green and red. On either side of the road, the control system must control a pedestrian light, a push button, and an optical indicator. Pushbutton activities on one side must also be indicated on the other. There is one light in each direction for the autos. The following figure depicts a more clear concept of the project.

 | <img src="./Images/System Block Diagram.PNG"> |
 |:--:| 
 | *System Block Diagram* |
 
 The following four main requirements were employed in the test verification process to implement the TLCS:
 
- Vehicle stopping
- Vehicle pre-crossing
- Vehicle crossing
- Vehicle post-crossing

The Finite State Machine (FSM) is implementated using State Flow Graphs follows the pattern as shown in the table below.

<table>
  
  <tr>
    <td colspan="5"><p align="center"><strong>Individual State Durations (sec) </strong></p> </td>
  </tr>
 
  <!--- <tr> (Comments)
  []: # <td rowspan="1"><b> States </b></td>
  []: # <td colspan="2"><b> Push button pressed</b> </td>
  []: # <td colspan="2"><b> Push button not pressed </b></td>
  []: # </tr> -->
 
  
  <tr>
    <td><p align="center"><b>States<b></p></td>
    <td><p align="center">Individual state time</p></td>
    <td><p align="center">Time elasped</p></td>
    <td><p align="center">Individual state time</p></td>
    <td><p align="center">Time elasped</p></td>
  </tr>
  
  
   <tr>
    <td>Vehicle Stopping</td>
    <td><p align="center">50</p></td>
    <td><p align="center">50</p></td>
    <td><p align="center">30</p></td>
    <td><p align="center">30</p></td>
  </tr>
     <tr>
    <td>Vehicle Pre-crossing</td>
    <td><p align="center">5</p></td>
    <td><p align="center">55</p></td>
    <td><p align="center">5</p></td>
    <td><p align="center">35</p></td>
  </tr>
     <tr>
    <td>Vehicle Crossing</td>
    <td><p align="center">30</p></td>
    <td><p align="center">1 min 25</p></td>
    <td><p align="center">30</p></td>
    <td><p align="center">1 min 05</p></td>
  </tr>
     <tr>
    <td>Vehicle Post-crossing</td>
    <td><p align="center">5</p></td>
    <td><p align="center">1 min 30</p></td>
    <td><p align="center">5</p></td>
    <td><p align="center">1 min 20</p></td>
  </tr>
</table>

According to above logic, FSM is developed in MATALAB/Simulink/Sate Flow Graphs as shown in below figure.

| <img src="./Images/FSM Design.PNG"> |
|:--:| 
| *FSM Design* |

The overview of the system that is executed and tested are given below.

| <img src="./Images/TLC Module.PNG"> |
|:--:| 
| *TLC Module* |

## Testing and Verfication

** Test 1 **

Thank you for visiting my account. I wish you a good day! 🙂
