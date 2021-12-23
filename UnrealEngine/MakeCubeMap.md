# Generate/make Cube Map HDR in Unreal Engine (Texture Cube HDR)

## Example of CubeMap texture

![image](https://user-images.githubusercontent.com/54003204/147298754-bb05fabb-6b75-4357-8035-5cb33c729cc0.png)

Can be used for example in Realistic windows with fake interiors

![image](https://user-images.githubusercontent.com/54003204/147298862-bd3ce8db-59a5-4ae6-8d95-f604e3619d22.png)


## Generate CubeMap

1. Load the interior scene you want to generate a cubemap from.

![image](https://user-images.githubusercontent.com/54003204/147299136-977f9de9-0eab-4e70-a5dd-dd8e8ec1c635.png)

2. Drag Scene Capture Cuba to your scene

![image](https://user-images.githubusercontent.com/54003204/147299177-8feecac4-b075-4592-b78a-0e8d19029bb3.png)

![image](https://user-images.githubusercontent.com/54003204/147299450-a24168ce-a380-41de-a3de-d9bc33a38e6e.png)


Create new asset - Cube Render Target 

![image](https://user-images.githubusercontent.com/54003204/147299462-d1dc703a-cb35-49f1-8de2-d7140d30be2c.png)

Select folder and set name 'renderCube' (You can use any name)

![image](https://user-images.githubusercontent.com/54003204/147299538-c7b0af9c-d4ce-4a5c-bfb5-7aa1947f2e77.png)

Open asset 'renderCube' and set resolution

![image](https://user-images.githubusercontent.com/54003204/147299844-3de4fb79-0421-4778-860d-7a5dde416075.png)


3. Set the "Scene Capture Cube" in right position in scene. The cube texture/map will be rendered automaticly.

4. Export asset 

![image](https://user-images.githubusercontent.com/54003204/147299729-d1350e52-30ff-4e55-8e48-212a28b7bc9a.png)

![image](https://user-images.githubusercontent.com/54003204/147300076-8af5dd73-5607-4531-b7a2-4e83ca81dbca.png)


## Import cube map to UE4

For example to use in asset 'Realistic windows with fake interiors'

1. Drag HDR file - exported before to UE4

![image](https://user-images.githubusercontent.com/54003204/147300367-f0c878b3-2bf8-4a9c-9e67-0ec09d8b8b9b.png)

2. In material instance change TextureCube to imported file 

![image](https://user-images.githubusercontent.com/54003204/147300504-0ba869ce-22f0-409a-b1ca-2e1fd1d9126d.png)
