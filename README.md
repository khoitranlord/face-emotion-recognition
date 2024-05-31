### Summary:
The repository contains a facial emotion recognition model using a CNN and optional mediapipe face landmarks for facial emotion prediction.

_________________

### To run the program
1) Install python 3.10
2) Install everything you need
   - `git clone https://github.com/khoitranlord/face-emotion-recognitionn.git`
   - `cd face-emotion-recognitionn`
   - `python -m venv venv`
   - Activate the virtual environment
     - `source venv/bin/activate`
   - `pip install -r requirements.txt`
   - `python -m spacy download en_core_web_lg`
   - `pip install torch`
3) `python setup.py`
4) `python run.py`
___________

* #### Image model:
    - The image is passed through a CNN model.
    - Landmarks are extracted from the image.
    - The CNN output and the landmarks are concatenated and passed through dense layers to get the emotion prediction.
