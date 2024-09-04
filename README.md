# Sviam.ai



# Virtual Clone System Prototype

## Project Overview

This project is a prototype for a virtual clone system capable of creating personalized avatars that can lip-sync to any given script. The avatars are customizable in terms of appearance, clothing, and voice tone, and the user has control over camera settings such as angles, lighting, and backgrounds.

---

## Setup Instructions

### 1. Prerequisites

- **Operating System**: Windows, macOS, or Linux
- **Python 3.x**: Install from [python.org](https://www.python.org/)
- **Node.js and NPM**: For handling the UI (if using web technologies)

### 2. Clone the Repository

```bash
git clone https://github.com/your-repo/virtual-clone-system.git
cd virtual-clone-system
```

### 3. Install Dependencies

- **Python Libraries**:
    ```bash
    pip install -r requirements.txt
    ```

- **Node.js Libraries** (if using a web-based interface):
    ```bash
    npm install
    ```

#### Dependencies:
- **Wav2Lip** (for lip-syncing)
- **Blender** or **Ready Player Me API** (for avatar customization)
- **DeepFaceLab** or **D-ID** (for facial mapping)
- **Text-to-Speech (Google TTS or Amazon Polly)** for voice generation
- **Unity or Three.js** (for camera control and rendering)

### 4. Set Up External APIs

If you are using Google Text-to-Speech or Amazon Polly, you will need to set up the relevant API keys. Refer to the following guides for setup:

- [Google Cloud TTS Setup](https://cloud.google.com/text-to-speech/docs/quickstart-client-libraries)
- [Amazon Polly Setup](https://docs.aws.amazon.com/polly/index.html)

---

## Usage Instructions

### Step 1: Input Data

- **Photos**: Upload a front-facing photo. This photo will be used to create the avatar.
- **Voice Recording**: Upload a voice recording (optional) or provide a text script for automatic speech generation using the built-in TTS engine.

### Step 2: Customize Avatar

- **Appearance**: Adjust facial features, hair, skin tone, and clothing options using the customization panel.
- **Voice Tone**: Use the tone control slider to modify the pitch and depth of the avatar's voice.

### Step 3: Camera Settings

- Select from preset camera angles (front, side, close-up).
- Adjust lighting and background options for a professional look.

### Step 4: Generate Video

Once all settings are configured, press the "Generate" button to create the final video. The system will process the input and generate a lip-synced video of the avatar speaking the script.

### Step 5: Output

The final output will be a video file (.mp4) with the virtual avatar lip-syncing the provided script. The video will feature customizable camera angles, lighting, and background settings.

---

## Customization

### Avatar Customization Options

- **Face and Body**: Customize the face (skin tone, hair, eye color) and clothing.
- **Voice**: Change the voice tone by adjusting pitch.

### Camera Customization Options

- **Camera Angles**: Select from preset options (front, side, or close-up).
- **Background**: Choose from a selection of virtual backgrounds or upload a custom image.
- **Lighting**: Adjust brightness, contrast, and shadows to achieve a professional video look.

---

## Troubleshooting

- **Lip-Syncing Issues**: Ensure that the audio file is clear and the face in the photo is well-lit and front-facing.
- **Voice Generation Errors**: Check that the TTS API is set up correctly with valid credentials.
- **Rendering Issues**: If using Blender or Unity, make sure the rendering environment is properly set up and dependencies are installed.

---

## Future Work

In future versions, we plan to introduce more advanced body movements, expressions, and full-body avatar options.
