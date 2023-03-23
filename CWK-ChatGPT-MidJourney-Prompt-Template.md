# CWK Midjourney Prompt Formula Guideline V0.1 - Object-Oriented Version - Experimental

Midjourney is an AI Art generator program uses cutting-edge technology to create images with a unique artistic style, and a midjourney prompt is a text phrase that the Midjourney Bot interprets to produce an image. A well-crafted prompt can help make unique and exciting images.

I need your assistance in creating midjourney prompts and I wanted you to help me in an object-oriented way.

Let's build a class hierarchy of midjourney prompts startiing with a generic class.

## Generic Prompt

This generic prompt class acts as the top-most class of this hierarchy.

When I just say 'midjourney prompt' or simply 'prompt', use the following formula:

* (Subject)
* (Content-Type: water color painting, water color sketch, lineart, 3d render, pencil drawing, movie poster, sticker, tattoo stencil, logo, icon, illustration, mockup, product shot, advertisement, pattern, oil, painting, acryl painting, infographic, cinematic still, movie poster, etc)
* (Style: In the Style of )
* (Color: sepia, monochrome color, blue and yellow, vibrant, muted, blue, yellow, red, etc)
* (Lighting: cinematic, dramatic, moody, bright, natural, artificial, dim dark, direct flashlight, blue light, from behind, volumetric, natural, octane render, a morning  scene with soft and warm light, a night scene with artificial light and neon signs, etc)
* (Perspective: portrait, close-up, medium close-up, extreme close-up, top down angle, full shot, wide shot, birds-eye view, worm's eye view, first-person, third-person, low-angle, high-angle, cowboy shot, medium full shot, full shot, dutch-angle, etc)

Optional properties:

* (Focal Length: 12MM, 24MM, 35MM, 50MM, 85MM, 135MM, 200MM, etc) 
* (F-Stop: f1.2, f1.4, f2.8, f8, etc)
* (Preferences: high detail)
* (Parameters: watermarks::-1 --ar 2:1 --q 1 --seed (a random number ranging from 0 to 4294967295))

This class does not use optional properties, but its descendants can. 

If its descendants does not specify a keyword from the optional properties, don't use it.

## Cinematic Prompt

Cinematic Prompt inherits the formula of Generic Prompt. 

When I just say 'cinematic prompt' or 'cine prompt', override only those properties of the specified keyword:

* 'Cinematic Still of (Subject)' overrides (Subject)
* '' overrides (Content-Type)
* 'Film By (Director: James Cameron, Denis Villeneuve, Park Chan-woo, etc)'' overrides (Style)
* (Focal Length) 
* (F-Stop)
* (Preferences)
* (Parameters)

Say yes if you understood and give me the examples of each prompt.
