<h2>Project Introduction</h2>
The aim of this project was, to build a prototype, showcasing the capabilities a Virtual F1 Attendance application would need and how it could look. The application in mind (Virtual F1 Attendance) would enable a User to watch a virtual F1 race as if he was attending the race at the racetrack, providing the needed immersion into the virtual world for an exhilarating experience.
<br></br>
In order to accomplish this, the choice of a suitable game engine for development needs to be determined. Given the growing popularity of NVIDIA's Omniverse and the increasing adoption of USD (Universal Scene Description) as a standard for 3D development applications, the decision was made to utilize Omniverse in conjunction with Unreal Engine 5. This choice will not only facilitate the creation of the prototype but also allow for testing the collaborative and co-simulation capabilities between Omniverse and Unreal Engine, as Omniverse provides a Connector for Unreal Engine (UE). 

As a prerequisite we recommend looking at the project <a href="https://dev.epicgames.com/community/learning/tutorials/e9EJ/unreal-engine-co-simulation-ue-and-omniverse-spaceverse-gtc-demo-return-on-experience">"Co-Simulation UE and Omniverse - "SpaceVerse" GTC demo - Return on Experience"</a>, as many parts of this project base on it as well as the idea for delving into co-simulation between Omniverse and Unreal Engine was sparked by this project.


<h2>Overview</h2>
This repository is split into 3 Folders. 

The OmniverseExtensions Folder holds the needed Omniverse Extensions to showcase the Virtual F1 Attendance Prototype (switching of viewport/position on the track) and also to showcase the concurrent simulation of the Animation in both Omniverse USD Composer as well as Unreal Engine. For both of these application we want to refer you to the <a href="https://github.com/itsthestranger/omni-virtual-f1-prototype/blob/main/Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report.pdf">Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report</a> for more information.
<br></br>
The USD Scenes Folder holds a compressed file containing 2 Scenes. One scene ("RB6_RedBullRing_Driving.usd"), where the racecar can be driven around the track and another scene ("RB6_RedBullRing_Animation_with_Cams.usda") holding the animation of the racecar driving around the track.
<br></br>
The UnrealEngineAssets folder containes the needed UAssets for the Demos as well as the modified Omniverse Plugin.


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
