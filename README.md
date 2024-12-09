# Edge TTS with Python: Threaded Text-to-Speech and Playback

This Python script demonstrates how to implement a threaded **Text-to-Speech (TTS)** system using the `edge_tts` library for speech generation and `pygame` for audio playback. The program supports concurrent TTS generation and playback while handling file management efficiently.

---

![image](https://github.com/user-attachments/assets/2b8cf079-e663-4ee4-b886-ab8750b85859)

## 🛠️ Features

- **Asynchronous TTS Generation**: Utilizes `edge_tts` for high-quality text-to-speech output.
- **Multi-threaded Implementation**: Separates TTS generation and playback into threads for better performance.
- **Audio Playback**: Plays the generated speech using the `pygame` library.
- **Robust File Management**: Includes a retry mechanism to safely handle temporary audio files.
- **Customizable Voice**: Supports Microsoft's neural voices (e.g., `en-AU-WilliamNeural`).

---

## 📋 Requirements

- **Python**: Version 3.7 or higher
- **Required Libraries**:
  - `edge-tts`: For TTS generation  
    Install it using:  
    ```bash
    pip install edge-tts
    ```
  - `pygame`: For audio playback  
    Install it using:  
    ```bash
    pip install pygame
    ```

---

## 🚀 Usage

### 1. Clone or Download the Script
Save the script as `edge_tts_threaded.py` or your preferred filename.

### 2. Run the Script
```bash
python edge_tts_threaded.py
```

### 3. Modify Input
Change the `text` variable in the script to customize the TTS output.

---

## 🧩 Code Overview

### Voice Configuration
The voice used is set with the variable `VOICE`. You can choose from various Microsoft voices. For example:
```python
VOICE = "en-AU-WilliamNeural"
```

### Key Functions
#### 1. **`remove_file(file_path)`**
Safely removes a temporary audio file with a retry mechanism.

#### 2. **`generate_tts(TEXT, output_file)`**
Asynchronous function to generate TTS using the `edge_tts` library.

#### 3. **`play_audio(file_path)`**
Plays the generated audio file using `pygame`.

#### 4. **`tts_with_playback(TEXT, output_file)`**
Combines TTS generation and playback in a threaded implementation for smooth operation.

---

## 🛠️ Example Code

```python
text = "Hello! This is a threaded implementation of Edge TTS using Python."
output_audio = "output.mp3"

# Run TTS and playback in threaded mode
tts_with_playback(text, output_audio)
```

---

## ⚙️ Advanced Enhancements

- **Voice Configuration**: Add dynamic input for voice selection.
- **GUI Integration**: Build a graphical interface using `Tkinter` or `PyQt`.
- **Logging**: Record errors and events for debugging.
- **Language Support**: Expand to support multilingual input for global users.

---

## 📜 License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute this script.

---

## 👤 Author

- **Name**: Anubhav Chaturvedi  
- 🐙 **GitHub**: [AnubhavChaturvedi-GitHub](https://github.com/AnubhavChaturvedi-GitHub)  
- 📺 **YouTube**: [NethyTech](https://www.youtube.com/channel/@nethytech)

---

## 🙌 Acknowledgments

- 📚 [Edge TTS Documentation](https://pypi.org/project/edge-tts/)
- 🎮 [Pygame Documentation](https://www.pygame.org/docs/)  
- 💡 Inspired by the open-source community.  

Let me know if you need further modifications! 🚀
