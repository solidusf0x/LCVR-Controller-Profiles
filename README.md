# LCVR Controller Profiles

This repo contains a list of input binding overrides that can be used to make different kind of controllers work correctly with the [Lethal Company VR mod](https://github.com/DaXcess/LCVR)

# Profiles

| Name      | Author                                 | Comment                                                                       |
| --------- | -------------------------------------- | ----------------------------------------------------------------------------- |
| `default` | [@DaXcess](https://github.com/DaXcess) | These are the default controller bindings that are included with the LCVR mod |

# Writing a custom profile

> This section is not yet finished

You can add a custom profile by either creating JSON files manually, or using the Unity Editor to create Input Action Assets, which you will have to export to a JSON file.

**Handy dandy resources**:
[Unity XR Input](https://docs.unity3d.com/Manual/xr_input.html)
[Input Common Usages](https://docs.unity3d.com/ScriptReference/XR.CommonUsages.html)

## Writing JSON manually

It is recommended to use the `default` profile as a baseline, which already contains valid input bindings in a valid format.

To change a binding: edit it's `path` key and change it to the binding of your choosing. If you know enough about Unity's Input System, you can also edit the `processors` key or use composites for more complex input binding (e.g. adding a binding that requires two inputs). Otherwise it is recommended to create these using a Input Action Asset inside of the Unity Editor.

## Using the Unity Editor

TODO

# Adding your profile

Fork this git repository, and add your variant of controller profiles.

Your controller profile should consist of two files: `lcvr_vr_inputs.json` and `lcvr_lc_inputs.json` (take a peek at the `default` profile to see how to set it up properly).

Place these inside of a directory with whatever name you want to give this profile. Please use lowercase names and replace spaces with underscores (`_`).

Next, update this README.md file and add your profile to the list.

Once everything is ready, create a pull request, and if everything checks out, it will be merged.
