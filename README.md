# Autodesk Inventor Thread Modeler

## Description

The Thread Modeler tool has been developed to allow Autodesk Inventor users to generate a realistic modeled equivalent thread based on an existing Inventor thread feature. 

Users are able to select an existing thread feature in the model, which the Thread Modeler then converts to a realistic 3D modeled thread based on the underlying thread feature properties.

Modeled threads are generated saving a lot of time and effort for the user when compared with a manual approach, bringing a higher degree of realism to your models.

Unfortunately the plugin from the autodesk [store](https://apps.autodesk.com/INVNTOR/en/Detail/Index?id=2540506896683021779&appLang=en&os=Win64) was depreciated around 2021 and no longer works for Inventor versions above 2020.

<img src="https://raw.githubusercontent.com/ThePieMonster/Autodesk-Inventor-Thread-Modeler/main/Sample/Sample.png" alt="drawing"/>

## Install

Copy the `ThreadModeler.bundle` plugin folder to your Autodesk Application Plugin folder.

Plugin folder: `C:\ProgramData\Autodesk\ApplicationPlugins`

## Issues

Currently in Inventor 2024, the thread modeler will overextend the created threads as shown in the below image. 

<img src="https://i.imgur.com/a8hG55D.png" alt="drawing" width="800"/>

<br/>

This can be fixed by editing the revolve sketch.

<img src="https://i.imgur.com/8C1TKcO.png" alt="drawing" width="800"/>

<br/>

By shorting the rectangle here we can fix the created 3D thread length. 

<img src="https://i.imgur.com/tHMEmz5.png" alt="drawing" width="800"/>

<br/>

Final result. 

<img src="https://i.imgur.com/p1cp9lp.png" alt="drawing" width="800"/>

## Development

Autodesk has a [handout](https://www.autodesk.com/autodesk-university/class/Creating-Add-Ins-Inventor-2018#handout) that can help you get started with plugin developement. 

The rundown is this:

- Install Visual Studio Community Edition

- Run `C:\Users\Public\Documents\Autodesk\Inventor 2024\SDK\developertools.msi`

- Open GitHub project solution
