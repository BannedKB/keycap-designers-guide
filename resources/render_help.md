# Guide to creating keycap renders:

1st step: Do the donut tutorial, found here: https://www.youtube.com/watch?v=TPrnSACiTJ4 to familiarize yourself with Blender and how it works.

2nd step: Lay out your kitting in http://www.keyboard-layout-editor.com/ to know what keys you will be using. 

3rd step: Go to #designer-resources and find the keycap models you need, be they Cherry, SA, or other profiles.

4th step: Import the models into a blender file.

5th step: Find the keys and rows you need, using your KLE (Keyboard Layout Editor) layouts you've made as a reference, and lay them out correctly. This can be done by setting your blender grids scale to .00473, and moving things around

6th step: UV map legends onto the keycaps. You can do this using this tutorial by @Frosty https://www.youtube.com/watch?v=ozS0gw0JAQ4&feature=youtu.be. There are legend files in #designer-resources , and #keyboard-render-kit in the Keycap Designer Discord.

7th step: Create your material for the keycaps. Different manufacturers and profiles have different textures, but this is usually accomplished in blender by attaching a Noise Texture, or a Voronoi texture node attached to a bump node, which you then attach to the normal node in your principled BSDF, and changing the values on them, making them rougher, shinier, bumpier, etc. (see attached photo)

8th step: Figure out your lighting. You should have color accurate lighting, at least for kitting renders, and make sure the light is not too bright or too dim. This is accomplished by using either 3 point lighting, an HDRI, like the Montreal HDRI Pack found here: https://www.maximeroz.com/hdri-free-pack, or using a Sky Texture node.

9th step: Render using as high samples as you can go, and if the end result is still noisy, use a denoiser such as  OpenImageDenoise in the render options of blender.

