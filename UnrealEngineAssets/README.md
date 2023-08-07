<h2>Overview</h2>

These files are the needed files for the USD Property readout in Unreal Engine and thus they are needed for the concurrent simulation showcase.

The files need to be moved to the "Content" Folder of your Unreal Engine Project. After moving these files into your "Content" Folder you simply need to use the "MyOmniverseStageActor.uasset" instead of the default "OmniverseStageActor" Actor. Therefore simply drag the "MyOmniverseStageActor.uasset" into the scene and add your .live file to the "USD" property of the Omniverse Stage Actor, as signalled in Figure below.

![Screenshot 2023-08-07 141124_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/2829d463-b123-4e15-a9b2-59a9a63ca70d)


Further you can look at the "MyOmniverseStageActor" Blueprint Class by opening it as displayed in the Figure below.

![Screenshot 2023-08-07 141341_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/3c002c86-0991-4763-bb88-dce167803f48)


When opening the "MyOmniverseStageActor" Blueprint Class you should see the same contents as presented in the Figure below. By default the "Event BeginPlay" Node is connected to the Node, which enables the readout of a float property of the underlying USD Scene. This can be tested in combination with the "RB6_RedBullRing_Driving.usd", as here the "Steer" property of the drivable vehicle is read out. An example of how this looks is shown here:

![Screenshot 2023-07-12 164248_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/f031b720-1ae6-404a-9be1-23a6d8f56910)


If you connect the "Event BeginPlay" Node to the "Concurrent Simulation" Node, this enables the triggering of the animation based on the underlying "activate" boolean value in the "RB6_RedBullRing_Animation_with_Cams.usda" scene. Thus the "Concurrent Simulation" Node functions as a listener, which then plays/pauses the animation based on the state of the underlying boolean property.

![Screenshot 2023-08-07 141416_edited (2)](https://github.com/itsthestranger/omni-virtual-f1-prototype/assets/11008552/f376132a-f631-4a59-bb51-326b3fbe6209)


<h4>Note:</h4>
For more information, please refer to the <a href="https://github.com/itsthestranger/omni-virtual-f1-prototype/blob/7ea0b955227409f05f484fd9236dff1f29cc9b23/Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report.pdf">"Virtual_F1_Prototype_and_Omniverse_UE_CoSim_Report"</a>.

