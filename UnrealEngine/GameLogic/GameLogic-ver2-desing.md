# Goorka Studio Unreal Engine Game Logic version 2 - design

## Types

### Linear 

StepChanger - class describe game step changing configuration (use in controlls like Checkpoint...)
 - NextStep - names of next game step
 - NextStepDelay - the delay [ms] after which the next step will be executed. (after triggered, delay [ms] and then change game step
 - SoundPosityve - 
 - SoundPositiveDelay - delay [ms] after positive sound played 
 - SoundNegative
 - SoundNegativeDelay - delay [ms] after positive sound played
 - LevelName - level that be openet on positive

ActiveSteps 
 - ActivityDelay - activity delay [ms], after a new step change. (After a new step change, delay [ms] and execute activity)
 - Steps - game steps separatet by ',' and allowed span separated by '-' examle: step2,step3,step4-step10, that activite control/component
  	  

## Controlls

 - Checkpoint - controll allowed, that change step when touched
    StepChanger: StepChanger
    Visiblity:ActiveSteps - when is visible and active
    
 - SetStepOnLevelBegin - control in editor
    StepName
  
 - VisibleOnStep - component 
    Visiblity:ActiveSteps
    
 - SnapPad - control where you snap 3d object (with SnapComponent)
    SnapId
    Visiblity:ActiveSteps
    StepChanger: StepChanger
    
 - SnapComponent
    SnapId
    
 - Timer - change step after [ms]
    Delay
    NextStep:NextStep
    ActiveSteps:ActiveSteps
    
  
 - PickableComponent - component allowed pick 3d object
  
  
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
