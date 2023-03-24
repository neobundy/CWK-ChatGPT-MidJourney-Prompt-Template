# Midjourney User Manual Edited By CWK

## What is Midjourney and Midjourney Prompt?

Midjourney is an AI Art generator program that create images with a unique artistic style.

A Midjourney Prompt is a short text phrase that the Midjourney Bot interprets to produce an image. The Midjourney Bot breaks down the words and phrases in a prompt into smaller pieces, called tokens, that can be compared to its training data and then used to generate an image. A well-crafted, well-weighted prompt can help make unique and exciting images.

To generate images, users use the /imagine command and type in a prompt; the bot then returns a set of images. 

## Prompt Structure

### Basic Prompts

A basic prompt can be as simple as a single word, phrase or emoji.

### Advanced Prompts

More advanced prompts can include one or more image URLs, multiple text phrases, and one or more parameters

#### Image Prompts

Image URLs can be added to a prompt to influence the style and content of the finished result. Image URLs always go at the front of a prompt.

#### Prompt Text

The text description of what image you want to generate. Well-written prompts help generate amazing images.

#### Parameters

Parameters change how an image generates. Parameters can change aspect ratios, models, upscalers, and lots more. 

## Prompting Notes

### Prompt Length

Prompts can be very simple. Single words (or even an emoji!) will produce an image. Very short prompts will rely heavily on Midjourney’s default style, so a more descriptive prompt is better for a unique look. However, super-long prompts aren’t always better. Concentrate on the main concepts you want to create.

### Grammar

The Midjourney Bot does not understand grammar, sentence structure, or words like humans. Word choice also matters. More specific synonyms work better in many circumstances. Instead of big, try gigantic, enormous, or immense. Remove words when possible. Fewer words mean each word has a more powerful influence. Use commas, brackets, and hyphens to help organize your thoughts, but know the Midjourney Bot will not reliably interpret them. The Midjourney Bot does not consider capitalization.

Midjourney Model Version 4 is slightly better than other models at interpreting traditional sentence structure.

### Focus on What you Want

It is better to describe what you want instead of what you don’t want. If you ask for a party with “no cake,” your image will probably include a cake. If you want to ensure an object is not in the final image, try advance prompting using the --no parameter.

### Think About What Details Matter

Anything left unsaid may suprise you. Be as specific or vague as you want, but anything you leave out will be randomized. Being vague is a great way to get variety, but you may not get the specific details you want.

Try to be clear about any context or details that are important to you. Think about:

Subject: person, animal, character, location, object, etc.
Medium: photo, painting, illustration, sculpture, doodle, tapestry, etc.
Environment: indoors, outdoors, on the moon, in Narnia, underwater, the Emerald City, etc.
Lighting: soft, ambient, overcast, neon, studio lights, etc
Color: vibrant, muted, bright, monochromatic, colorful, black and white, pastel, etc.
Mood: Sedate, calm, raucous, energetic, etc.
Composition: Portrait, headshot, closeup, birds-eye view, etc.

### Use Collective Nouns

Plural words leave a lot to chance. Try specific numbers. "Three cats" is more specific than "cats." Collective nouns also work, “flock of birds” instead of "birds.”

I need your assistance in creating midjourney prompts and I wanted you to help me in an object-oriented way.

Let's build a class hierarchy of midjourney prompts startiing with a generic class.

## Explore Prompting

Even short single-word prompts will produce beautiful images in Midjourney's default style, but you can create more interesting personalized results by combining concepts like artistic medium, historical periods, location, movie, infographic, vector graphics, and more.

### Pick A Medium

Break out the paint, crayons, scratchboard, printing presses, glitter, ink, and colored paper. One of the best ways to generate a stylish image is by specifying an artistic medium.

prompt example: /imagine prompt <any art style> style cat

### Get Specific

More precise words and phrases will help create an image with exactly the right look and feel.

prompt example: /imagine prompt <style> sketch of a cat

### Time Travel

Different eras have distinct visual styles.

prompt example: /imagine prompt <decade> cat illustration

### Emote

Use emotion words to give characters personality.

prompt example: /imagine prompt <emotion> cat

### Get Colorful

A full spectrum of possibilities.

prompt example: /imagine prompt <color word> colored cat

### Enviromental Exploration

Different environments can set unique moods.

prompt example: /imagine prompt <location> cat

## Parameter List

Parameters are options added to a prompt that change how an image generates. Parameters can change an image's Aspect Ratios, switch between Midjourney Model Versions, change which Upscaler is used, and lots more.

Parameters are always added to the end of a prompt. You can add multiple parameters to each prompt.

### Basic Parameters

Aspect Ratios

--aspect, or --ar Change the aspect ratio of a generation.

Chaos

--chaos <number 0–100> Change how varied the results will be. Higher values produce more unusual and unexpected generations.

No

--no Negative prompting, --no plants would try to remove plants from the image.

Quality

--quality <.25, .5, 1, or 2>, or --q <.25, .5, 1, or 2> How much rendering quality time you want to spend. The default value is 1. Higher values cost more and lower values cost less.

Seed

--seed <integer between 0–4294967295> The Midjourney bot uses a seed number to create a field of visual noise, like television static, as a starting point to generate the initial image grids. Seed numbers are generated randomly for each image but can be specified with the --seed or --sameseed parameter. Using the same seed number and prompt will produce similar ending images.

Stop

--stop <integer between 10–100> Use the --stop parameter to finish a Job partway through the process. Stopping a Job at an earlier percentage can create blurrier, less detailed results.

Style

--style <4a, 4b or 4c> Switch between versions of the Midjourney Model Version 4

Stylize

--stylize <number>, or --s <number> parameter influences how strongly Midjourney's default aesthetic style is applied to Jobs.

Uplight

--uplight Use an alternative "light" upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image is less detailed and smoother.

Upbeta

--upbeta Use an alternative beta upscaler when selecting the U buttons. The results are closer to the original grid image. The upscaled image has significantly fewer added details.

## Aspect Ratios

The --aspect or --ar parameter changes the aspect ratio of the generated image. An aspect ratio is the width-to-height ratio of an image. It is typically expressed as two numbers separated by a colon, such as 7:4 or 4:3.

A square image has equal width and height, described as a 1:1 aspect ratio. The image could be 1000px × 1000px, or 1500px × 1500px, and the aspect ratio would still be 1:1. A computer screen might have a ratio of 16:10. The width is 1.6 times longer than the height. So the image could be 1600px × 1000px, 4000px × 2000px, 320px x 200px, etc.

The default aspect ratio is 1:1.

--aspect must use whole numbers. Use 139:100 instead of 1.39:1.

The aspect ratio impacts the shape and composition of a generated image.

Some aspect ratios may be slightly changed when upscaling.

### Common Midjourney Aspect Ratios

--aspect 1:1 Default aspect ratio.
--aspect 5:4 Common frame and print ratio.
--aspect 3:2 Common in print photography.
--aspect 7:4 Close to HD TV screens and smartphone screens.

## How to Change the Aspect Ratio

### Use Aspect Ratio Parameters

Add --aspect <value>:<value>, or --ar <value>:<value> to the end of your prompt.

## Seeds
 
 The Midjourney bot uses a seed number to create a field of visual noise, like television static, as a starting point to generate the initial image grids. Seed numbers are generated randomly for each image but can be specified with the --seed or --sameseed parameter. Using the same seed number and prompt will produce similar ending images.

--seed accepts whole numbers 0–4294967295.
--seed values only influence the initial image grid.
--seed values Model Versions 1, 2, 3, test, and testp are non-deterministic and will produce similar, not identical, images.

Using the same prompt+seed+parameters in Model Versions 4, 5 and niji will produce identical images.

### Seed Parameter

If no Seed is specified, Midjourney will use a randomly generated seed number, producing a wide variety of options each time a prompt is used.

### Sameseed Parameter

--seed values create a single large random noise field applied across all images in the initial grid. When --sameseed is specified, all images in the initial grid use the same starting noise and will produce very similar generated images.

--sameseed accepts whole numbers 0–4294967295.
--sameseed is only compatible with Model Versions 1, 2, 3, test, and testp.

### How To Change Seed Numbers

Use the --seed or --sameseed Parameter.

Add --seed <value> or --sameseed <value> to the end of your prompt.


## Stylize

This Midjourney Bot has been trained to produce images that favor artistic color, composition, and forms. The --stylize or --s parameter influences how strongly this training is applied. Low stylization values produce images that closely match the prompt but are less artistic. High stylization values create images that are very artistic but less connected to the prompt.

--stylize's default value is 100 and accepts integer values 0–1000.

### How to Switch Stylization Values

Add --stylize <value> or --s <value> to the end of your prompt.

## Tile
 
The --tile parameter generates images that can be used as repeating tiles to create seamless patterns for fabrics, wallpapers and textures.
--tile works with Model Versions 1, 2, 3 and 5.
-
-tile only generates a single tile. Use a pattern making tool like this Seamless Pattern Checker to see the tile repeat.

### How to Use the Tile Parameter

Add --tile to the end of your prompt.

