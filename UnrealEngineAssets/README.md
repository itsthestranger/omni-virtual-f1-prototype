<h2>Overview</h2>
We provide 2 options regarding the creation of an Unreal Engine project capable of reading-out the underlying USD properties of a USD file.  

<h3>Option 1</h3>
The folder "Option1" holds a compressed Unreal Engine project, which you simply need to extract and open. 

To do this extract the .zip file and once extracted double-click the "OmniverseUECoSim.uproject" file. After doing this you should be prompted with a message stating, that modules are missing and that they need to be rebuild. Click "Yes".

![Screenshot 2023-08-09 105937_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/732f356d-137d-4ffd-bdd0-bb46d54be794)

The recompliation takes a while, but after some time the project should open and you should see the "MyOmniverseStageActor" Blueprint Class in the "Content" Folder.

![Screenshot 2023-08-09 110314_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/68cd0b73-3778-4cf4-9090-f801c95fccf0)

To ensure everything works correctly, open the "MyOmniverseStageActor" Blueprint Class, right-click in the Event Graph and search for "Omniverse UE". Here you now should see the functions displayed in the Figure below, which means everything works correctly.

![Screenshot 2023-08-08 120543_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/2f0bfcce-da4f-42f1-8757-bbb5283f5bec)


<h3>Option 2</h3>
The second option we provide enables the usage of custom Unreal Engine Project i.e. with the second option you can modify your own Unreal Engine Project to enable the read-out of underlying USD properties in Unreal Engine. Therefore the folder "Option2" holds all necessary files to achieve the read-out of USD Properties in Unreal Engine. 

The .uasset files are the needed files for the USD Property readout in Unreal Engine and thus they are needed for the concurrent simulation showcase.

The Plugins.rar contains the Plugins folder, which holds the modified Omniverse Plugin and after creating your Unreal Engine Project (make sure you have C++ enabled) you simply need to move this Plugins folder to the root of your project files. As an example refer to the Figure below.

![Screenshot 2023-08-08 120838_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/f8d11a27-3bea-4946-8ec5-8a8b855de830)


The .uasset files need to be moved to the "Content" Folder of your Unreal Engine Project, as displayed in the Figure above. After moving these files into your "Content" Folder you simply need to use the "MyOmniverseStageActor.uasset" instead of the default "OmniverseStageActor" Actor. 

To ensure everything works correctly you can look at the "MyOmniverseStageActor" Blueprint Class by opening it.


![Screenshot 2023-08-07 141416_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/f376132a-f631-4a59-bb51-326b3fbe6209)

After opening the "MyOmniverseStageActor" Blueprint Class you should see the same contents as presented in the image above and when right-clicking in the Event Graph and searching for "Omniverse UE" you should again see the custom functions for getting and setting USD Properties (Figure below).

![Screenshot 2023-08-08 120543_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/2f0bfcce-da4f-42f1-8757-bbb5283f5bec)


<h4>MyOmniverseStageActor Overview</h4>

By default the "Event BeginPlay" Node is connected to the Node, which enables the readout of a float property of the underlying USD Scene. This can be tested in combination with the "RB6_RedBullRing_Driving.usd", as here the "Steer" property of the drivable vehicle is read out. An example of how this looks is shown here:

![Screenshot 2023-07-12 164248_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/f031b720-1ae6-404a-9be1-23a6d8f56910)


If you connect the "Event BeginPlay" Node to the "Concurrent Simulation" Node, this enables the triggering of the animation based on the underlying "activate" boolean value in the "RB6_RedBullRing_Animation_with_Cams.usda" scene. Thus the "Concurrent Simulation" Node functions as a listener, which then plays/pauses the animation based on the state of the underlying boolean property.


<h4>Note:</h4>
For more information, please refer to the <a href="https://github.com/itsthestranger/omni-virtual-f1-prototype/blob/main/Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report.pdf">"Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report"</a>.

