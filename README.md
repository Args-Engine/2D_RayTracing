# Guided Learning Minor CMGT
During my minor I will be trying to make a 2D raytracer.

## Current implementations

The first iteration will be raycasting in 2D on CPU using ray (or infinite line)-linesegment collision (which has been done correctly since the new ray-line collisions in [commit #7](https://github.com/Args-Engine/guided_learning_jelle/commit/456535cf3064aefc30efec5833dc101fbe7620bd)). Furthermore, when a ray collides with a line segment it needs to reflect (since [9th commit](https://github.com/Args-Engine/guided_learning_jelle/commit/1cf8d5df85e64ad3bf2d2957b0a84e8364fc5067)). The reflected ray should now have the color of the original ray (which came from the light) and the line segment it hit (since the [6h commit](https://github.com/Args-Engine/guided_learning_jelle/commit/e09867a5d0fe60dd52dfb2b56c6108c57f07a193)). From here it is important that images will have collision as well. We don't want to setup all the line segment colliders for images our selves, so since [September 7, 2020, commit #21](https://github.com/Args-Engine/guided_learning_jelle/commit/ce45a6671c7017396611aa6c0898943ee07a8229) the basics of the image to line segment interpreter work.

# Future implementations
In the future more colliders for rays need to be added, for example ray-circle collision. This way more accurate collisions and reflections can be achieved. Image to line segments needs to be improved, since certain details are not yet recognized. Also gabs of empty pixels will also not be recognized yet. 

# Relevance
The industry is working towards improving real-time raytracing in 3D. 3D real-time raytracing has of course been done on a vew games. However 2D raytracing in the same way, with global illumination and lighting up sprites, has not been done. Raycasting has been done in 2D for player view, or to find the area which a light would light up, but the light would not be used to light up the walls, or sprites it would hit. Next to 2D not being rendered using raytracing, 2D being rendered with normal and height maps has also not been done for too long. In my opinion 2D games are still relevant, especially for indie games. Some of my favorite games are 2D games. However 3D games are more used in triple-A companies and therefore get more research and usually ending up looking better. I think applying some 3D technology on a 2D game, can be really interesting.
