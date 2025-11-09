# AI-Generated Music

Project that aims to generate synthetic music with AI having a local music dataset of songs of different genres.

## 🎵 Project Components

### 1. Music Dataset Creator Notebook (`music_dataset_creator.ipynb`)

A comprehensive Jupyter notebook that allows you to:
- Import local MP3 files from a folder
- Extract audio features (tempo, MFCCs, spectral features, etc.)
- Create a structured dataset for AI model training
- Visualize feature distributions
- Export dataset in multiple formats (CSV, JSON, Pickle)

#### Getting Started with the Notebook

1. **Install Required Dependencies:**
```bash
pip install librosa pandas numpy matplotlib scipy jupyter
```

2. **Launch Jupyter Notebook:**
```bash
jupyter notebook music_dataset_creator.ipynb
```

3. **Add Your Music Files:**
   - Create a folder named `music_files` in the project directory
   - Add your MP3 files to this folder
   - Update the `MUSIC_FOLDER_PATH` variable in the notebook if using a different location

4. **Run the Notebook:**
   - Execute each cell sequentially
   - The notebook will process your MP3 files and create a dataset
   - View visualizations and statistics about your music collection

#### Features Extracted

The notebook extracts over 50 audio features including:
- **Tempo**: Beats per minute
- **MFCCs**: 13 Mel-frequency cepstral coefficients (mean and std)
- **Spectral Centroid**: Brightness of the sound
- **Spectral Rolloff**: Shape of the signal
- **Zero Crossing Rate**: Rate of sign changes
- **Chroma Features**: 12 pitch class distributions
- **RMS Energy**: Root mean square energy

### 2. Web Frontend (`app/index.html`)

A professional, modern web interface with:
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Interactive Navigation**: Smooth scrolling menu with active state highlighting
- **Hero Section**: Eye-catching introduction with gradient background
- **Features Section**: Six feature cards showcasing capabilities
- **Interactive Demo**: Buttons to simulate dataset creation, training, and generation
- **Stats Section**: Key metrics displayed with animated numbers
- **Contact Section**: Professional footer with contact form and social links
- **Modern UI**: Dark theme with gradient accents and smooth animations

#### Viewing the Web Frontend

1. **Open the HTML file:**
   - Navigate to the `app` folder
   - Open `index.html` in your web browser

2. **Use a Local Server (Recommended):**
```bash
cd app
python -m http.server 8000
```
   - Then open `http://localhost:8000` in your browser

## 📁 Project Structure

```
AI-generated-music/
├── music_dataset_creator.ipynb  # Jupyter notebook for dataset creation
├── app/
│   └── index.html               # Web frontend
├── music_files/                 # Place your MP3 files here (create this folder)
├── README.md                    # Project documentation
├── LICENSE                      # License file
└── .gitignore                   # Git ignore file
```

## 🚀 Quick Start Guide

### Step 1: Set Up Your Environment

```bash
# Clone the repository
git clone https://github.com/pintamonas4575/AI-generated-music.git
cd AI-generated-music

# Install dependencies
pip install librosa pandas numpy matplotlib scipy jupyter
```

### Step 2: Prepare Your Music Files

```bash
# Create a folder for your music files
mkdir music_files

# Copy your MP3 files to this folder
cp /path/to/your/music/*.mp3 music_files/
```

### Step 3: Create Your Dataset

```bash
# Launch Jupyter Notebook
jupyter notebook music_dataset_creator.ipynb

# Run all cells to process your music and create the dataset
```

### Step 4: Explore the Web Interface

```bash
# Navigate to the app folder
cd app

# Start a local web server
python -m http.server 8000

# Open http://localhost:8000 in your browser
```

## 🎯 Next Steps

After creating your dataset, you can:

1. **Train an AI Model**: Use the extracted features to train a music generation model (RNN, LSTM, Transformer, etc.)
2. **Music Classification**: Build a model to classify songs by genre or mood
3. **Music Recommendation**: Create a recommendation system based on audio features
4. **Generate New Music**: Train a generative model to create original compositions

## 📊 Dataset Output

The notebook generates several output files:

- `music_dataset.csv`: Dataset in CSV format
- `music_dataset.json`: Dataset in JSON format
- `music_dataset.pkl`: Dataset in Pickle format (for Python)
- `feature_names.txt`: List of all extracted features
- `feature_distributions.png`: Visualization of feature distributions

## 🛠️ Requirements

- Python 3.7+
- librosa
- pandas
- numpy
- matplotlib
- scipy
- jupyter (for running the notebook)

## 📝 License

This project is licensed under the terms specified in the LICENSE file.

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📧 Contact

For questions or suggestions, please use the contact form on the web interface or open an issue on GitHub.

---

Built with ❤️ for music creators and AI enthusiasts
