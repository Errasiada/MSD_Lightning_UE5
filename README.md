# MSD_Lightning_UE5

This practice was made with Unreal Engine 5. The idea is to create a main level and add several feautures that will be detailed below.

First of all is creating an exterior scenario. In my case, I used several pictures I made as a reference and then I started creating the scene.

The player is a ThirdPersonController that is able to move and jump around the scene. The landscape was made adding a terrain, several high-ground areas and low-ground areas to make it feel more realistic, several trees simulating a grove and a water-like area as an ocean. Some base materials were made for this: 1. Ground base, 2. Ground with grass layer, 3. Ground and ice for the mountains. Next is adding a global light as a sun.

These are some references I used for the landscape.

![IMG_20211216_080033](https://user-images.githubusercontent.com/114673717/212701802-9d8140b5-f78e-4a24-95b0-9ead21657dd9.jpg)

![IMG_20220508_164610](https://user-images.githubusercontent.com/114673717/212701667-32a7e7d0-f955-48e6-8649-0e9c4411ce10.jpg)

These are some inGame samples

![22577c8d21d55b813ac70058e27ec6d4](https://user-images.githubusercontent.com/114673717/212701102-b6a5e48f-62ad-4907-8e48-459a4baf853c.jpg)

![7709afcba5deb280bcef619758315541](https://user-images.githubusercontent.com/114673717/212701007-0a44f1e4-7358-4cb3-a889-791d2c87a070.png)


Secondly I built the main cottage. This cottage was built using several Assets from Quixel Bridge, searching for a medieval-rustic style objects and furniture so it was easier to simulate a tyical Canarian house. The cottage has an old door and a big opened window, to let the sun light enter inside the building.

![closeup](https://user-images.githubusercontent.com/114673717/212700911-dbf53582-b526-498c-aef7-1cda50663c3f.jpg)

![back window](https://user-images.githubusercontent.com/114673717/212700932-d5b4b98a-8bad-4f1c-b127-941d94ca4ea0.jpg)


There is a path to the house entrance that works as a guide for the player. The house is placed in a nearby field after the grove and between a bunch of mountains. Several objects were added near the entrance to give that antique looking. A mist was added to the house interior using a Niagara System of Hanging Particles and modifying its values.

![house and path](https://user-images.githubusercontent.com/114673717/212700842-68ba10ab-63e6-48af-bb6a-1c2a15c68e34.png)

Mist (Niagara System)

![image](https://user-images.githubusercontent.com/114673717/212701341-7f38f47c-0b83-4de0-8e85-bd49dd62a156.png)



After that I added a main table inside the building with the main object, an Old Jar, that the player is supposed to interact with using a "pick up" system. I used a spotlight over the object to recreate the artificial light, changing its values such as bloom,intensity, color, radius, etc. This spotlight guides the player to the old jar. Once the player collisions with the object, it will be destroyed.

![interior spotlight](https://user-images.githubusercontent.com/114673717/212700950-54c66538-a930-418e-86ea-cbf6619edafe.jpg)

![table_object](https://user-images.githubusercontent.com/114673717/212700803-eca5cf54-96e7-4aca-907e-8d1031584e26.png)


Here's the object blueprint for the pick-up action.

![old jar](https://user-images.githubusercontent.com/114673717/212729825-6e83a684-52ad-4325-ad3e-02ed6ad80917.png)


After picking the Old Jar a new object will spawn in the map: a Wheelbarrow. This object will appear in an small open area just behind the house. The player can see trough the house window the spot.

Reference image:

![IMG_20211216_080025](https://user-images.githubusercontent.com/114673717/212701975-b8cca755-7411-4912-879a-abcd50c3dd86.jpg)

inGame object:

![spawn item](https://user-images.githubusercontent.com/114673717/212701550-e6af0cc9-82fd-45b1-8e15-9b3efa200a88.png)

Wheelbarrow blueprint:

![wheelbarrow](https://user-images.githubusercontent.com/114673717/212730120-95f0c9d8-861f-4486-a568-bcd050582577.png)

Finally, once the player interacts with the object, the character will be destroyed. Here is the level blueprint for that action.

![map](https://user-images.githubusercontent.com/114673717/212730011-7985d359-baf9-438d-bb79-de747e4b3e1a.png)


