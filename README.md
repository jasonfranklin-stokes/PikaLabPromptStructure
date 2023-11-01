This text has been designed to be given to a an AI agent to undeerstand how to use PIKALABS. 

# PIKA GUIDE - 1.11.2023

## PIKALABS

Pika Labs offers a text-to-video creation platform. To use:

Access: Visit Pika Labs website and join their Discord server with a Discord account.
Channels: Use the ‘generate’ channel for video creation.
Video Creation: DM Pika Bot with 'create' and your prompt.
Reference Images: Upload to guide video's starting frame.
Feedback: Use thumbs down and 'regenerate' for revisions.
Editing: 'Remix' to modify prompts.
Parameters: Customize with FPS, GSC, neg, AR, seed, and camera controls.
Camera: Pan, zoom, and rotate for dynamic videos.

### PARAMETERS IN PIKA LABS:

#### Frames per second:
- **Parameter:** `-fps##`
  - **Use for:** adjusting the frames per second, the higher, the more smoother your video becomes
  - **Values:** 8-24 (default is 24)

#### Motion:
- **Parameter:** `-motion#`
  - Represents the intensity of the movement, the higher the value the more intense the motion will become in the video
  - **Values:** set from 1 to 4 → 1 is default

#### Guidance scale:
- **Parameter:** `-gs##`
  - The higher the value the more related it is to the text prompt
  - **Values:** use between 8 and 24 (Pika default is 12)

#### Negative prompt:
- **Parameter:** `-neg`
  - Means negative prompt indicating the content you don't want to appear in the video
  - **Example:** `-neg morphing, erratic fluctuation in motion, noisy, bad quality, distorted`

#### Aspect ratio:
- **Parameter:** `-ar #:|`
  - This is for adjusting aspect ratio - The width:height of a video
  - **Values:** 16:9, 9:16, 1:1, 4:5, or the default from your image if you use: image to video

#### Seed:
- **Parameter:** `-seed ###`
  - **Use for:** More consistent generation. Currently fixing seed ONLY guarantees consistency when both prompt and negative prompt are unchanged
  - **Accepts:** Numbers (default is random)
  - **Example Prompt:** `/create prompt: this is an example of a prompt -seed 123456789`
  - **Note:** seed number of a generated video can be found at the end of its file name

### CAMERA MOVEMENTS IN PIKA LABS:

#### Camera movement:
Controlling the camera movement in your video clip. You can choose to zoom, pan, or rotate. Remember, you can only use one of these at a time, and they can't be combined.

##### ZOOM IN:
Adjust the camera's distance from the subject. You can either zoom in or zoom out, depending on your preference.
- **Parameter:** 
  - `-camera zoom in`
  - `-camera zoom out`

##### PAN:
Adjust the camera to display more of the background, keeping the main subject fixed. Choose from pan up, pan down, pan left, or pan right, or use a combination like pan up left or pan down right.
- **Parameter:** 
  - `-camera pan up` / `-camera pan down`
  - `-camera pan left` / `-camera pan right`
  - `-camera pan up left` / `-camera pan up right`
  - `-camera pan down left` / `-camera pan down right`

##### ROTATE:
Reposition the camera to orbit the object, or tilt the frame to a Dutch angle. Options include rotating clockwise (cw), counterclockwise (ccw), or anticlockwise (acw).
- **Parameter:** 
  - `-camera rotate clockwise` / `-camera rotate cw`
  - `-camera rotate counterclockwise` / `-camera rotate ccw`
  - `-camera rotate anticlockwise` / `-camera rotate acw`

### My personal tips for using parameters and camera movements:
- I've attempted to add camera movements/parameters after creating a regular video, but this often leads to a significant change in the motion. To achieve the desired result, you can either use the rerun button a few times or simply add your camera movements when you initially upload the image.
- You've got to appreciate a good shot. If it excites you when you first see it, go with that shot. All images often have some kind of issues, so you might end up trying 100 versions without success. But if you immediately feel like, "Yes, this is it," then use that video.

### BASIC PROMPTING FOR TEXT TO IMAGE APPS & TEXT TO VIDEO IN PIKA LABS:

#### Basic prompt structure:
**Example1:**
| Style | Subject / action | Shot type | Scene description | lighting | Aspect ratio & style |
|-------|------------------|-----------|-------------------|----------|----------------------|
| Cinematic | Female with astronaut helmet | Close up shot | Mars desert with sand and storm | Peach light | --ar 16:9--style raw |

**Example2:**
| Style | Subject / action | Shot type | Scene description | lighting | Aspect ratio & style |
|-------|------------------|-----------|-------------------|----------|----------------------|
| Photography | A young African woman with a dog | Establishing shot | A beach with blue sea | Sunlight | --ar 1: --style raw |

#### Negative prompts examples:
- `-neg morphing, erratic fluctuation in motion, noisy, bad quality, distorted, poorly drawn, blurry, grainy, low resolution, oversaturated, lack of detail, inconsistent lighting`
