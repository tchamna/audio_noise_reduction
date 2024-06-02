# Audio Noise Reduction Application

This is a Streamlit-based application for reducing noise in MP3 audio files. It allows users to select a folder containing MP3 files, specify the level of noise reduction, and process the files to reduce noise.

## Features

- Select a folder containing MP3 files.
- Specify the noise reduction proportion.
- Automatically process all MP3 files in the folder.
- Save the denoised files in a new folder.


## Installation

1. **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2. **Create a virtual environment (optional but recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Run the Streamlit application:**

    ```bash
    streamlit run audio_noise_removal_streamlit.py
    ```

2. **In the Streamlit web interface:**

    - Enter the path to the folder containing MP3 files.
    - Use the slider to select the noise reduction proportion (0.0 to 1.0). A higher value removes more noise but may affect audio quality.
    - Click the "Start Noise Reduction" button to begin processing.

3. **The application will:**

    - Read all MP3 files in the specified folder.
    - Apply noise reduction to each file.
    - Save the denoised files in a new subfolder named `denoised_<proportion>` within the original folder.


4. **View the completion message:**

    ![Completion Message](images/completion_message.png)

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Streamlit](https://streamlit.io/) for providing an easy-to-use framework for creating web applications.
- [pydub](https://github.com/jiaaro/pydub) for audio processing.
- [noisereduce](https://github.com/timsainb/noisereduce) for noise reduction.

