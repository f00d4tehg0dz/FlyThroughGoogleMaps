# FlyThroughGoogleMaps

[DEMO GAME](https://drive.google.com/file/d/1qxqKGCxKJKcA0gsqPmUE0R--dc5TqCkt/view?usp=share_link)
Hold down Left Click to fly around
WSAD for Throttle Up/Down, Left, and Right
Spacebar to open Postcard. *Sometimes you need to mouse cursor over the entered text twice and hit enter key to activate.*



Inspired from the great work that reddit user /u/bakkernils [where he linked ChatGPT and Google Maps 3D Tiles together to generate a cool flythrough of Google Maps in Unreal Engine](https://www.reddit.com/r/unrealengine/comments/13m0st3/i_connected_the_new_google_maps_3d_tiles_chatgpt/)

This is a loose recreation of his work to give to the OpenSource community

# Steps

1. Make sure to drop the OpenAIApi-5.1.1.zip in your UE5.x Plugins folder and activate in UE5.x
2. I used [Dynamic Volumetric Sky](https://www.unrealengine.com/marketplace/en-US/product/dynamic-volumetric-sky?sessionInvalidated=true) to handle the sky. $19.99. You can safely delete if not wanted
3. I leveraged [Responsive_MenuUI_Template](https://www.unrealengine.com/marketplace/en-US/product/responsive-menu-template-ui) for the Menu system. $4.99. You can safely delete if not wanted
4. Make sure to install Cesium plugin, its free in The Unreal Marketplace and activate in UE5.x
5. OpenAPI Key can be entered in ThirdPerson/Blueprints/BP_PlayerController/BeginPlay/Set Open AIApi Key
6. Google API Key can be entered in Maps/Maps/Map.map under Cesium World Terrain > https://tile.googleapis.com/v1/3dtiles/root.json?key=XXXXXX