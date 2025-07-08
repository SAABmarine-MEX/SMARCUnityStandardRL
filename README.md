# SMARC Unity Standard

Welcome to the Standard (Built-in Engine) version of SMARC Unity.
This project has all of the dependencies configured and installed in order to showcase the [SMARC Unity Assets package](https://github.com/martkartasev/SMARCUnityAssets) with minimal effort.

## SAABmarine-MEX Fork
### *BlueROV2 with residual dynamics modelling and DRL*

This fork contains the work from the [SAABmarine-MEX](https://github.com/SAABmarine-MEX) project. It has created a BlueROV2 simulation with residual dynamic modelling and DRL capabilities.

The scenes for this work have been structured as follows bellow (the .meta files are not included for easier visual interperation). The corresponding assets repo can be found [here](https://github.com/SAABmarine-MEX/SMARCUnityAssets).

```
SMARCUnityStandardRL/Assets/Scenes/Dev/BlueROV2/
├── BrovAsko.unity (From old project, the hk mechatronics project)
├── BrovEmpty.unity (General BlueROV2 in empty environment)
├── BrovRLTankEval.unity (RL evaluation)
├── BrovRLTankTrain.unity (RL training)
├── BrovTank.unity (General BlueROV2 in the water tank)

├── Models/ (RL models)
│   ├── Brov-1190164.onnx
│   ├── Brov-1198264.onnx
│   ├── Brov-1328315.onnx
│   ├── Brov-1499754.onnx
│   ├── Brov-2230496.onnx
│   ├── Brov-2354632.onnx
│   ├── Brov-463136.onnx
│   ├── Brov-525754.onnx
│   ├── Brov-669668.onnx
│   ├── Brov-6doftranslational.onnx
│   ├── Brov-999623.onnx
│   ├── Brov.onnx
│   └── Brov-tether1.onnx

└── ResidualDynamic/ 
    ├── PriorBrovEmpty.unity (Prior is the default sim)
    └── RealBrovEmpty.unity ("Real" is made different to the default sim to test residual training without real data)
```


## New to Unity?

------

If you have not used unity before I suggest trying out a few tutorials from https://learn.unity.com/

To get started, I suggest you familiarize yourself with the editor from: https://learn.unity.com/tutorial/explore-the-unity-editor-1#

### I cannot see anything!

If you want to jump in quickly to see the sim, follow the next few steps.

1. In the Project Window (tab at the bottom) open: Scenes/WaterSimulation.Unity
2. In the central panel, click on Scene. This is the "Editor" window. The "Game" window is simply a camera that has been set up into the scene.
3. In the Hierarchy (panel on the left side), double click on SAM to pan to it.
4. Click the Play button

From here you should be able to move SAM around using the arrow keys and WASD. You might want to drag and drop the Game window (you can split the view), so you can see both the Scene and Game windows in parallel.
