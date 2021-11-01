# Character Creator to Blender Rigify to UnrelEngine - Animation workflow

1. Create model

![image](https://user-images.githubusercontent.com/54003204/139698775-8f002c91-e739-4b9e-b197-b56c2282ef72.png)

2. Export to UE4

![image](https://user-images.githubusercontent.com/54003204/139698987-2844f98e-c498-45b4-8c9a-7394ffc8ce1e.png)

![image](https://user-images.githubusercontent.com/54003204/139701198-22320c62-4dbd-4178-ba8b-d51e7d122f09.png)


I suggest a file name convention modelName_pose_exportFromTo.fbx
example:
kobieta_apose_fromCCtoUe (CC - Character Creator, Ue - Unreal Engine ). When You edit and export model from blender you can use kobieta_tpose_formBtoUe ...

Character Creator allow also export to blender, but don't use it if you want to export model to UE.

3. Import to blender

![image](https://user-images.githubusercontent.com/54003204/139701780-795709bc-7d51-4863-8887-c03b631a581c.png)

I suggest create collection for new model - it will be easy using rigify when you use more rigs in one scene

![image](https://user-images.githubusercontent.com/54003204/139702130-16499254-1da9-46c6-b860-e2c6da7e7412.png)

4. Remove rig  from imported armature, and scale all object by 0.01 and move character to ground, and apply all transform (Ctrl+A)

![image](https://user-images.githubusercontent.com/54003204/139702795-90cd37bb-35fc-4fe3-a5de-0568cfe61c28.png)

5. Add Rigify metarig and in edit mode pose pone in corect position


