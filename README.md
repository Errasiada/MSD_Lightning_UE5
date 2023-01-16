# MSD_Lightning_UE5

This practice was made with Unreal Engine 5. The idea is to create a main level and add several feautures that will be detailed below.

First of all is creating an exterior scenario. In my case, I used several pictures I made as a reference and then I started creating the scene.

The player is a ThirdPersonController that is able to move and jump around the scene. The landscape was made adding a terrain, several high-ground areas and low-ground areas to make it feel more realistic, several trees simulating a grove and a water-like area as an ocean. Some base materials were made for this: 1. Ground base, 2. Ground with grass layer, 3. Ground and ice for the mountains. Next is adding a global light as a sun.

These are some references I used for the landscape.
(insertar fotos base del entorno y referencias y jugador)

Secondly I built the main cottage. This cottage was built using several Assets from Quixel Bridge, searching for a medieval-rustic style objects and furniture so it was easier to simulate a tyical Canarian house. The cottage has an old door and a big opened window, to let the sun light enter inside the building.

There is a path to the house entrance that works as a guide for the player. The house is placed in a nearby field after the grove and between a bunch of mountains. Several objects were added near the entrance to give that antique looking. A mist was added to the house interior using a Niagara System of Hanging Particles and modifying its values.

After that I added a main table inside the building with the main object, an Old Jar, that the player is supposed to interact with using a "pick up" system. I used a spotlight over the object to recreate the artificial light, changing its values such as bloom,intensity, color, radius, etc. This spotlight guides the player to the old jar. Once the player collisions with the object, it will be destroyed.

Here's the object blueprint for the pick-up action.

After picking the Old Jar a new object will spawn in the map: a Wheelbarrow. This object will appear in an small open area just behind the house. The player can see trough the house window the spot.

Finally, I introduced a transparent material as a box collider around the wheelbarrow that allows the player to end the game.

