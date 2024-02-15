# Unity

Virtual environments are built using Unity and are versioned using several repositories and git submodules. Please consult the "Getting started" section to install a toplevel repository.

## Submodules

In the Assets folder of the Unity project, there are several git submodules that implement different modular aspects of the simulator:

- `vr_scenes` : This is the main submodule. It contains the scenes to simulate, and most static (non-moving) assets. Static assets are benches, light posts, etc., and they are prefabs that include their geometry, textures and colliders. The scenes generally make references to other contents from the `vr_dynamic_objects`, `vr_street_lights` and `vr_user` submodules.
- `vr_dynamic_objects` : Dynamic objects such as pedestrians and cars, as prefabs that include their geometry, textures, colliders, animators and scripts.
- `vr_street_lights` : Configurable street light and road prefabs that allow interaction with the user with a push button.
- `vr_user` : A game object with basic physics, one main camera and colliders that represents the user in a first-person point of view. This is also where we put the interfacing scripts with external devices, such as DBox, haptics, motion analysis.


## Updating (pull)

Use the "Pull with submodules" custom action that you created in "Getting started".

## Editing

When working on the game, one must make sure that the new files (scripts, textures, etc.) added to a scene are placed in the correct folder, so that they will be added to the right repository.

## Committing

To commit the changes, start by commiting and pushing every change to the submodules. Then, commit and push the changes to the main repository.
