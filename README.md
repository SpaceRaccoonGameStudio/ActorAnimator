# ActorAnimator
# What is it?
**ActorAnimator** is a plugin that allows you to animate the components of the actors using curves and splines. With this plugin, you can easily create smooth and realistic animations that can be used in various projects, including games, architectural renderings, and others.

# Features

* Animate location by curves
* Animate location by internal splines (inside actor)
* Animate location by external splines (link any external actor with spline component)
* Animate scale by curves
* Animate rotation by curves
* Animate light color by curves
* Animate light intensity by curves
* Animate light temperature by curves
* Animate location by wind source (experimental)
* Create custom animation blueprints for any additional logic
* Create presets for reusing animations for any count of actors
* In any time pause/stop/reverse/change play speed for any animations
* Use animation contexts for extend animation logic
* Auto-play with delay/contexts
* Animate any actors placed to level (with some limitations)
* Combinate animations

# How it is work?

* You add a component to any actor
* Set up animations for each component (based on SceneComponent)
* Start animations using blueprints or autoplay (delayed start is supported)
* The component enable tick and creates a pool of animations for processing based on animation fragments (using the CDO version of the classes)
* In a tick, each fragment is processed and the object transformation / or any additional data is changed at the output
* The result of all animation fragments is summed by default, which allows you to combine different sets of animation fragments
* When animation fragments finish playing they are removed from the processing queue
* When the queue is empty, the tick of the component turns off

# Demo project

[Click to download](https://drive.google.com/drive/folders/1RpsGlOxJuXJXH9qz6R3vsVLfQi4WA3z6)

[Click to watch demo overview](https://www.youtube.com/watch?v=ltEAlfIhgAo)

# Example project

[Click to download](https://drive.google.com/drive/folders/1gdHLp2W7--clUQg_rnfmPyicdMbNvKX7)

# FAQ

Q: **What platforms are supported?**

A: Now it is Win32,Win64, Mac, Linux, Android, IOS - tested & worked. Potentially it should work on any platform. If you have any problems with platforms - please write me, I  will be fixt it


# Support

If you have any additional questions or suggestions, do not hesitate to express them. You can

do it through our official discord group or via email

**Discord** : [Click to join](https://discord.gg/4FtCJnMuxb)

**Email** : [support@space-raccoon.com](mailto:support@space-raccoon.com)
