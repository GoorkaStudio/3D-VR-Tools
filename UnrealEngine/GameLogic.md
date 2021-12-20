# Unreal Engine 4 - Game logic

## Types

StepChanger
  NextStep - names of next step
	NextStepDelay - delay [ms] after new step will be set
	SoundPosityve - 
	SoundPositiveDelay - delay [ms] after positive sound played 
	SoundNegative
	SoundNegativeDelay - delay [ms] after positive sound played
  LevelName - level that be openet on positive
  
NextStep - 
  Decision1StepName - default decision next step
  Decision2StepName
  Decision3StepName
  Decision4StepName
  
ActiveSteps 
  Delay - how long [ms] after step change set activity
  Steps - steps separatet by ',' and allowed span separated by '-' examle: step2,step3,step4-step10
  	

## Controlls

  Checkpoint - controll allowed, that change step when touched
    StepChanger: StepChanger
    Visiblity:ActiveSteps - when is visible and active
    
  SetStepOnLevelBegin - control in editor
    StepName
  
  VisibleOnStep - component 
    Visiblity
    
  SnapPad - control where you snap 3d object (with SnapComponent)
    SnapId
    Visiblity
    StepChanger
    
  SnapComponent
    SnapId
    
  PickableComponent - component allowed pick 3d object
