
🧠 Custom Image Classifier (Tkinter + PyTorch)

A modern desktop application for training and using your own image classification model — no advanced ML experience required.

Built with PyTorch, Torchvision, and a sleek Tkinter GUI.

✨ Features
📂 Classify single images or entire folders
🏷️ Create and manage your own custom classes
🧠 Transfer learning using ResNet-18 backbone
⚡ Fast training with feature extraction
📊 Real-time training progress & logs
🖼️ Live image preview with predictions
🎨 Modern dark-themed UI
🧱 How It Works
Uses a pretrained ResNet-18 model as a feature extractor
Freezes backbone weights (no heavy training needed)
Trains a custom fully connected head layer on your classes
Stores:
Model weights → custom_head.pth
Class metadata → custom_classes.json
📦 Installation
pip install torch torchvision pillow
🚀 Usage

Run the app:

python your_script_name.py
🧪 Workflow
1. Add Classes
Click "+ Add Class"
Enter class name
Select a folder with training images

👉 Images will be copied into:

custom_classes/<class_name>/
2. Train Model
Add at least 2 classes
Click "Train"

Training runs for:

EPOCHS = 30
3. Classify Images
Single Image
Browse or paste image path
Click "Classify"
Folder
Select folder
Click "Classify Folder"
📁 Project Structure
.
├── images/                 # Default test images
├── custom_classes/        # Training data (auto-created)
│   ├── class1/
│   └── class2/
├── custom_head.pth        # Trained model
├── custom_classes.json    # Class labels
├── main.py                # Your script
⚙️ Configuration

Inside the script:

EPOCHS = 30
LR = 0.01
INPUT_SIZE = (224, 224)

You can tweak:

Training epochs
Learning rate
Image preprocessing
🖼️ Supported Image Formats
.jpg, .jpeg
.png
.bmp
.gif
.webp
⚠️ Notes
You must train the model before classification
Minimum 2 classes required
More images = better accuracy
Works best with clear, consistent datasets
💡 Tips for Better Results
Use 20–100 images per class
Keep backgrounds consistent
Avoid mixing very different object types in one class
Use varied lighting & angles
🔧 Future Improvements (Ideas)
🔁 Incremental training
📊 Accuracy metrics
💾 Export/import datasets
🌐 Web version (Flask/Streamlit)
🧠 Support for larger models (ResNet50, EfficientNet)
👨‍💻 Author

Created by JP

<img width="1076" height="822" alt="Custom Image Classifier created" src="https://github.com/user-attachments/assets/6a414f31-fd1b-4b08-a184-5bcbc7e4641a" />



