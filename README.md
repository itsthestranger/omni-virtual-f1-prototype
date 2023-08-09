<h1>Omniverse and Unreal Engine Co-Simulation for a Virtual F1 Attendance Prototype</h1>

<h2>Project Introduction</h2>
The aim of this project was, to build a prototype, showcasing the capabilities a Virtual F1 Attendance application would need and how it could look. The application in mind (Virtual F1 Attendance) would enable a User to watch a virtual F1 race as if he was attending the race at the racetrack, providing the needed immersion into the virtual world for an exhilarating experience.
<br></br>
Given the growing popularity of NVIDIA's Omniverse and the increasing adoption of USD (Universal Scene Description) as a standard for 3D development applications, the decision was made to utilize Omniverse in conjunction with Unreal Engine 5. Apart from building a prototype for a Virtual F1 Attendance application we utilize the Omniverse UE Connector to first create a live connection between the two engines and then go further by modifying the Unreal Engine Omniverse Plugin to enable the live read-out of underlying USD Properties. This read-out of underlying USD properties in Unreal Engine enables us to achieve concurrent animation in both applications.
<br></br>
For a detailed explanation of all implemented features please refer to the <a href="https://github.com/itsthestranger/omni-virtual-f1-prototype/blob/main/Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report.pdf">Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report</a>.

<h2>Repo Overview</h2>
This repository is split into 3 Folders. 


The OmniverseExtensions Folder holds the needed Omniverse Extensions to showcase the Virtual F1 Attendance Prototype (switching of viewport/position on the track) and also to showcase the concurrent simulation of the Animation in both Omniverse USD Composer as well as Unreal Engine. For both of these application we want to refer you to the <a href="https://github.com/itsthestranger/omni-virtual-f1-prototype/blob/main/Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report.pdf">Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report</a> for more information.
<br></br>
The USD Scenes Folder contains 2 Scenes. One scene ("RB6_RedBullRing_Driving.usd"), where the racecar can be driven around the track and another scene ("RB6_RedBullRing_Animation_with_Cams.usda") holding the animation of the racecar driving around the track.
<br></br>
The UnrealEngineAssets folder containes 2 options to test the USD-Property readout in Unreal Engine. Option 1 provides a Unreal Engine Project, which can be opened and tested right away and Option 2 provides all needed files to modify an existing Unreal Engine Project.


<h2>Tech Requirements</h2>

<h3>Program Stack</h3>
The project was developed using Omniverse USD Composer (formerly known as Omniverse Create) and Unreal Engine by utilizing the Omniverse UE Connector and the Omniverse Local Nucleus Service. For a quick overview of the used program versions, refer to the table below.
<br></br>

<table>
  <tr>
    <th>Program</th>
    <th>Version</th>
  </tr>
  <tr>
    <td>Omniverse USD Composer</td>
    <td>2022.3.3</td>
  </tr>
  <tr>
    <td>Omniverse UE (5.1) Connector</td>
    <td>201.1.244</td>
  </tr>
  <tr>
    <td>Local Nucleus Service</td>
    <td>2022.4.2</td>
  </tr>
  <tr>
    <td>Unreal Engine</td>
    <td>5.1.1</td>
  </tr>
</table>

<h3>System Requirements</h3>
For the implementation of the prototype using Omniverse USD Composer, it is recommended to have at least an RTX 2080 GPU. The minimum GPU requirement is any RTX GPU with 6GB of VRAM.

In terms of CPU requirements, both the minimum and recommended specifications call for an Intel i7 or AMD Ryzen CPU. The minimum specifications require a minimum of 4 cores, while it is recommended to have 8 cores.
Regarding RAM, Omniverse USD Composer requires a minimum of 16GB, with 32GB being recommended for optimal performance.

For our project, the system used was in line with the recommended system requirements. It consisted of an RTX 2080 GPU, an Intel i7 8700 CPU, and 32GB of RAM.
