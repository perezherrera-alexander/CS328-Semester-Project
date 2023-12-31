# CS328-Semester-Project

Unity Version: 2022.3.9f1 (LTS)

### Version 0.6.2 (12/15/2023)
- Incresed music volume

### Version 0.6.1 (12/15/20230)
- Fixed issue where when recieving health on enemy kill, health would go above max health
- Fixed issue where the wizard boss's bullets would collider with the boss itself
- Removed settings button from main menu

### Version 0.6.0 (12/14/2023)
- Added 2 new enemies
    - Ghost
    - Minion (Unused)
- Added Wizard boss to level 2
- Completed level 2 design & logic
- Fully implemented beam staff
    - Fires a continuous beam of energy that can hit multiple enemies
- Added weapon switching (Press 1 or 2)
- Added win logic & screen to level 2
- Fixed various bugs

### Version 0.3.0 (12/1/2023)
- Added 3 new enemies
    - Skeleton
    - Goblin
    - Reanimated Suit of Armor
- Added Skeleton King boss to level 1
- Compelted level 1 design & logic
- Fully implemented mana mechanic
    - Mana is now used when casting spells
    - Mana regenerates over time
    - Killing enemies restores mana
- Added spells/powerups (Press Q or E)
- Added art for enemies
- Added music to menu and level 1
- Added sounds effects for shooting, dashing, and death

### Version 0.2.3 (11/9/2023)
- Redid dash mechanic
    - Now features a cooldown
    - Added a dash bar to the UI
- Updated level 1 geometry
    - Not yet complete but getting there
- Refactored "PlayerController.cs"
    - Created helper functions for getting the direction to the mouse from the player
    - Now caluclatng these values once in FixedUpdate() and passing them as arugments to where they are needed (so that we aren't calculating them multiple times per frame)

### Vesion 0.2.2
- Added Invisibility and Haste spells
    - Invisibility makes the player invisible to enemies
    - Haste increases the player's movement speed by double
- Created Invisibility animation, having trouble implementing, will come back to it


### Vesion 0.2.1
- Added dash mechanic to player controller
    - Not entirely happy with the implementation. There is a better way to do this, will revist later.

### Version 0.2.0 
- Updated Player prefab so that movement speed is now on a different scale
- Adjusted player speed and bullet speed to that the player does not outrun the bullets
- Fixed an issue where the Level 2 button would load level 1

### Version 0.1.5
- Added new temporary geometry to levels 1 & 2.

### Version 0.1.4
- Player now looks in mouse direction
- Added bullet prefab and sprite
- Player now can shoot

### Version 0.1.3
- Reformatted layout of scripts to script file
- Added an animation folder
- Added a sprite folder
- Added UI overlay
    - Displays current health
    - Displays current mana
- Added Pause Menu functionality
    - Can pause and unpause the game
        - Stops the game in background
    - Can exit to the main menu
    - Can exit the game

### Version 0.1.2
- Redid the player movement script to utilize RigidBody2D.movePosition() instead of transform.position
    - This should avoid a jittering issue when colliding with walls
- Added a camera controller script to the main camera
    - It just simply follows the player around
- Created a wall (with collision) to build levels with
- Made prefabs out of these GameObjects to allow for easy level creation
- Added these prefabs to the two exisitng levels with some basic geometry to differentiate them

### Version 0.1.1
- Added Main Menu scene, functionality, and UI
    - Allows switching between scenes and exiting the game
- Created level select scene
    - Allows switching between levels and going back to the main menu
- Updated player movement to be able to use WASD keys as well as arrow keys