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

<table>
  
   <tr>
    <td colspan="5"><p align="center"><strong>Individual State Durations (sec) </strong></p> </td>
  </tr>
  
  <tr>
    <td rowspan="1"><p align="center"><b> States </p></b></td>
    <td colspan="2"><p align="center"><b> Push button pressed </p></b> </td>
    <td colspan="2"><p align="center"><b> Push button not pressed </p></b></td>
  </tr>
  
  <tr>
    <td></td>
    <td>Individual state time</td>
    <td>Time elasped</td>
    <td>Individual state time</td>
    <td>Time elasped</td>
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
