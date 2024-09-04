
# SViam.ai: Virtual Avatar Clone System

SViam.ai is a prototype for creating a virtual avatar clone that can lip-sync to a given script with customizable features such as clothing, appearance, and voice tone. The focus is on rendering the upper body of the avatar in a professional setting.

## Features

- **Lip-Syncing**: The avatar accurately lip-syncs to the provided audio input.
- **Customizable Avatar**: Adjust the avatar’s clothing, appearance, and voice tone based on user input.
- **Camera Settings**: Modify camera angles, lighting, and background for professional output.
- **Steady Motion**: No full-body movements, only focused on upper-body animation.

## Setup and Dependencies

### Requirements

- **Python 3.x**
- **Google Colab or Local Python Environment** (with GPU recommended)
- **Libraries and Frameworks**:
  - TensorFlow or PyTorch (for lip-syncing and avatar models)
  - OpenCV for image processing and camera settings
  - Blender (optional, for 3D rendering)
  - ffmpeg for processing audio and video
  - Wav2Lip or similar models for lip-syncing
  - GAN models (e.g., StyleGAN) for avatar generation (optional)
  - TTS tools (e.g., Google Text-to-Speech, Tacotron2) for voice synthesis

### Installation

You can run SViam.ai directly in Google Colab or set it up locally.

#### 1. **Google Colab Setup**

- Clone the repository in Colab:
  ```bash
  !git clone https://github.com/thisisvk45/SViam.ai
  ```

- Install dependencies:
  ```bash
  !pip install -r requirements.txt
  ```

#### 2. **Local Setup**

- Clone the repository:
  ```bash
  git clone https://github.com/thisisvk45/SViam.ai
  cd SViam.ai
  ```

- Install dependencies using pip:
  ```bash
  pip install -r requirements.txt
  ```

- Ensure that you have a compatible GPU for rendering and lip-syncing tasks.

## Usage

### Inputs

- **Photo**: Upload a front-facing image of the person you want to create the avatar for. This image will be used for generating the face of the avatar.
- **Voice**: Upload an audio file or use the text-to-speech functionality to generate the voice.

### Running the Lip-Syncing Model

In the Colab notebook (or local environment), run the lip-syncing script:

```python
from lip_sync_module import sync_lips
sync_lips(photo='input/photo.jpg', audio='input/audio.wav')
```

### Avatar Customization

- **Clothing and Appearance**: You can modify the avatar’s clothing and facial features using the `avatar_customization` module.

```python
from avatar_customization import customize_avatar
customize_avatar(photo='input/photo.jpg', outfit='casual', hair='short', tone='neutral')
```

- **Voice Tone**: You can change the tone of the voice using the `tts_customization` function.

```python
from voice_customization import change_tone
change_tone(audio='input/audio.wav', tone='deep')
```

### Adjusting Camera Settings

Modify camera angles and lighting using the `camera_settings` module:

```python
from camera_settings import set_camera
set_camera(angle='front', lighting='soft', background='professional')
```

### Outputs

The prototype will generate a video file of the avatar delivering the script. You can download the final output from Colab or your local environment.

## Customization Options

You can control the following customization options for your avatar:

- **Clothing**: Select different outfits such as `casual`, `formal`, or `creative`.
- **Appearance**: Adjust hair length, skin tone, and facial features.
- **Voice Tone**: Adjust the voice tone to `high-pitch`, `neutral`, or `deep`.
- **Camera Settings**: Modify the angle (e.g., front, side) and lighting (soft, dramatic, etc.).

## Future Features

- **Emotion Detection**: Add facial expressions based on the script's emotional tone.
- **Real-time Processing**: Move toward real-time avatar lip-syncing.
- **Background Removal**: Implement automatic background removal or dynamic background changes.

---

## Example Workflow

1. Upload your photo and voice input files.
2. Customize the avatar’s appearance, clothing, and voice tone.
3. Adjust camera settings for a professional look.
4. Generate the video and download the final output.


