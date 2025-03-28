Overview
The AI Comic Crafter is a web application that generates a 4-panel comic strip based on a user-provided story prompt. It utilizes advanced AI models for text generation and image creation, specifically leveraging the Mistral 7B model for text and Stable Diffusion for image generation.

Features:
-Generate a short story based on a prompt.
-Create retro cartoon-style images for each panel of the comic.
-Display the generated story and images in a user-friendly interface.

System Requirements:
Local System Configuration
-To run this code locally, you will need the following system configuration:

Operating System: Windows, macOS, or Linux
-GPU: NVIDIA GPU with CUDA support (recommended for better performance)
-RAM: At least 16 GB (32 GB recommended for larger models)
-Python: Version 3.7 or higher
-CUDA: Version compatible with your GPU (if using GPU acceleration)

Required Libraries:
The following libraries need to be installed, which can be listed in a requirements.txt file:
-transformers
-diffusers
-torch
-matplotlib
-bitsandbytes
-gradio

Steps to Run on Google Colab:
1. Open Google Colab: Go to Google Colab.
2. Create a New Notebook: Click on "File" > "New Notebook".
3. Install Required Libraries: Copy and paste the following code into a cell and run it:

>>!pip install -q -r requirements.txt

4. Copy the Code: Copy the entire code provided in this repository into a new cell in the Colab notebook.
5. Set Hugging Face Token: Replace the hf_token variable in the code with your Hugging Face token. You can obtain a token by creating an account on Hugging Face.
6. Run the Code: Execute the cell containing the code. After a few moments, the Gradio interface will launch.
7. Interact with the App: Enter a story prompt and click "Generate Comic" to see the generated comic strip.

Steps to Run Locally:
1. Install Python: Ensure you have Python 3.7 or higher installed. You can download it from python.org.
2. Set Up a Virtual Environment (Optional): It is recommended to create a virtual environment to manage dependencies.

>>python -m venv comic_crafter_env
>>source comic_crafter_env/bin/activate  # On Windows use `comic_crafter_env\Scripts\activate`

3. Install Required Libraries: Use pip to install the required libraries:

>>pip install -r requirements.txt

4. Copy the Code: Copy the entire code provided in this repository into a Python file (e.g., comic_crafter.py).
5. Set Hugging Face Token: Replace the hf_token variable in the code with your Hugging Face token.
6. Run the Code: Execute the Python file (terminal / Command prompt):

python comic_crafter.py

7. Access the App: After running the code, a local server will start. Open the provided URL (usually http://127.0.0.1:7860) in your web browser to access the Gradio interface.
8. Interact with the App: Enter a story prompt and click "Generate Comic" to see the generated comic strip.

Troubleshooting:
1. CUDA Errors: Ensure that your GPU drivers and CUDA toolkit are correctly installed and compatible with the version of PyTorch you are using.
2. Library Installation Issues: If you encounter issues while installing libraries, ensure that you have the latest version of pip and try upgrading it:

>>pip install --upgrade pip