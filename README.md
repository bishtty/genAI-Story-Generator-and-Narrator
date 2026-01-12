# Story Generator 📸 -> 📖

Hi there! I built this little app because I thought it would be cool to take a bunch of random photos and let AI weave them into a proper story. It basically looks at your images, figures out what's happening, and writes a narrative for you. Plus, it reads the story out loud so you don't even have to read it yourself!

I used Python and Streamlit for the web interface, and under the hood, it's powered by Google's new Gemini models (specifically `gemini-2.5-flash-lite`) to do the creative writing.

## What it actually does

*   **Upload Photos:** You can drop in anywhere from 1 to 10 images.
*   **Pick a Vibe:** Want a mystery? A fairy tale? A sci-fi thriller? You just pick the genre from the dropdown.
*   **AI Magic:** It sends your images to Gemini, which writes a story connecting them all together.
*   **Listen to it:** It uses Google's Text-to-Speech to generate an audio file of the story automatically.

## How to run it

If you want to try this out on your own machine, here is what you need to do:

### 1. Get the code
Clone this repo (or just download the files):
```bash
git clone <your-repo-url>
cd storyGenerator
```

### 2. The Setup
You'll need Python installed. Then, grab the libraries I used:
```bash
pip install -r requirements.txt
```

### 3. API Key
Since this uses Google's Gemini, you need an API key. It's free to get one from [Google AI Studio](https://aistudio.google.com/).
Once you have it, create a file named `.env` in this folder and paste it in like this:
```env
GOOGLE_API_KEY=your_actual_api_key_here
```

### 4. Launch it! 🚀
Run this command:
```bash
streamlit run app.py
```
Your browser should open up automatically. Just upload some pics and hit the generate button.

## The Code
*   `app.py`: This is the main file that runs the Streamlit UI.
*   `story_generator.py`: This handles the calls to Gemini and the text-to-speech stuff.

Enjoy! Let me know if you make any cool stories with it.
