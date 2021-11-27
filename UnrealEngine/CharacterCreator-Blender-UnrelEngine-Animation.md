# Character Creator to Blender Rigify to Unreal Engine - Animation workflow

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

![image](https://user-images.githubusercontent.com/54003204/139707593-ec4a6054-3135-49a7-84fb-55250c88f910.png)

![image](https://user-images.githubusercontent.com/54003204/139707777-541be6de-42ba-4ea6-a6e3-674f9ad7e599.png)

Parent rig with object (Ctrl+P)

![image](https://user-images.githubusercontent.com/54003204/139707998-48d4a20d-ef38-4d61-99d6-0c8d0a5ca58d.png)

Corect weight paint 

![image](https://user-images.githubusercontent.com/54003204/139708795-2c0cf430-c804-4bf3-b08d-5091d6649348.png)

6. Multiple rigify rig - adding another rigify rig

![image](https://user-images.githubusercontent.com/54003204/139738706-27b33a77-02a5-4b7c-8289-3c26c853ac80.png)

![image](https://user-images.githubusercontent.com/54003204/139749995-a1068886-3695-4a01-81ce-7e50e067fa6b.png)



