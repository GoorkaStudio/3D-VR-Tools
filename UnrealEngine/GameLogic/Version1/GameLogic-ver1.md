# Goorka Studio Unreal Engine Game Logic version 1

Download and totorial
https://github.com/GoorkaStudio/3D-VR-Tools/blob/main/UnrealEngine/GameLogic/Version1/Tutorial-GoorkaGameLogic.md

## Controlls

  Checkpoint - controll allowed, that change step when touched
    StepChanger: StepChanger
    Visiblity:ActiveSteps - when is visible and active
    
  SetStepOnLevelBegin - control in editor
    StepName
  
  VisibleOnStep - component 
    Visiblity:ActiveSteps
    
  SnapPad - control where you snap 3d object (with SnapComponent)
    SnapId
    Visiblity:ActiveSteps
    StepChanger: StepChanger
    
  SnapComponent
    SnapId
    
  Timer - change step after [ms]
    Delay
    NextStep:NextStep
    ActiveSteps:ActiveSteps
    
  
  PickableComponent - component allowed pick 3d object
