# AI Voice Assistant with Multimodal RAG

This project is an AI Voice Assistant utilizing Retrieval-Augmented Generation (RAG) with multimodal capabilities. The assistant allows users to upload an image and interact with it by asking questions through voice input. The assistant responds with both text and audio answers, making it versatile for various industries such as customer support, education, healthcare, and more.

## Features

- **Multimodal Interaction**: Upload images and ask questions via voice.
- **Text and Audio Responses**: Get answers in both text and spoken form.
- **Versatile Applications**: Ideal for industries like healthcare, customer service, education, etc.
- **Advanced AI Models**: Powered by the latest AI models like LLAVA for image-to-text and Whisper for speech recognition.

## Screenshot

![image](https://github.com/user-attachments/assets/71400933-c1db-4295-9a03-63798b7fd800)


## Getting Started

### Prerequisites

- **Python 3.7+**
- **NVIDIA GPU** (Recommended: T4 for free-tier usage on Colab, V100 for faster processing)

### Installation

1. **Clone the repository** or upload the `.ipynb` file to Google Colab.

2. **Select GPU**: 
   - On Google Colab, go to `Runtime` > `Change runtime type`.
   - Select `GPU` and choose `T4` if you're using the free tier, or `V100` if available.

3. **Install dependencies**:
   - Run the following command in your Colab notebook to install the required dependencies:
     ```python
     !pip install -r requirements.txt
     ```
   - If you're installing manually, include the following in your `requirements.txt` file:
     ```txt
     torch==2.0.1
     transformers==4.37.2
     bitsandbytes==0.41.3
     accelerate==0.25.0
     whisper
     gradio==3.33.1
     gTTS==2.2.4
     nltk==3.8.1
     Pillow==9.2.0
     numpy==1.24.2
     requests==2.31.0
     ```

4. **Download Models**:
   - **Whisper**: Install Whisper from the GitHub repository:
     ```python
     !pip install -q git+https://github.com/openai/whisper.git
     ```
   - **LLAVA Multimodal Model**: Use the model `"llava-hf/llava-1.5-7b-hf"` for image-to-text generation.

### Running the Assistant

1. **Upload Image**: Use the Gradio interface to upload an image.
2. **Ask Questions**: Speak your question into the microphone.
3. **Get Responses**: Receive both text and audio answers from the assistant.

## Use Cases

- **Customer Support**: Analyze product images and answer customer inquiries.
- **Education**: Provide detailed descriptions and explanations of visual content.
- **Healthcare**: Assist in interpreting medical images with verbal and written guidance.

## Contribution

Contributions are welcome! Feel free to fork the repository and submit pull requests.

## License

This project is licensed under the MIT License.

---

Enjoy using the AI Voice Assistant with Multimodal RAG for your innovative applications!
