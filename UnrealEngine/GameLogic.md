# Unreal Engine 4 - Game logic
GoorkaStudio Game Logic ver. 1.0

## Types

### Linear 

StepChanger
  NextStep - names of next step
  NextStepDelay - delay [ms] after new step will be set
  SoundPosityve - 
  SoundPositiveDelay - delay [ms] after positive sound played 
  SoundNegative
  SoundNegativeDelay - delay [ms] after positive sound played
  LevelName - level that be opened on positive

ActiveSteps 
  Delay - how long [ms] after step change set activity
  Steps - steps separated by ',' and allowed span separated by '-' example: step2,step3,step4-step10
  	
### Branch

StepBranch
  Decision1:StepChanger
  Decision2:StepChanger
  Decision3:StepChanger
  Decision4:StepChanger

  
NextStepDescription - 
  Decision1StepName - default decision next step
  Decision2StepName
  Decision3StepName
  Decision4StepName
  

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
    Visibility:ActiveSteps
    StepChanger: StepChanger
    
  SnapComponent
    SnapId
    
  Timer - change step after [ms]
    Delay
    NextStep:NextStep
    ActiveSteps:ActiveSteps
    
  
  PickableComponent - component allowed pick 3d object
