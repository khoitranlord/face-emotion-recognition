### Summary:
The repository contains a facial emotion recognition model using a CNN and optional mediapipe face landmarks for facial emotion prediction.
_______________
### Sample output for the model:
#### Face model:

<table>
  <tr>
    <td><img src="display_files/disgust_2.png" width="300" style="margin-right: 10px;"></td>
    <td><img src="display_files/disgust_emotion.jpg" width="200" style="margin-right: 10px;"></td>
    <td><img src="display_files/disgust_grad_cam.jpg" width="200" style="margin-right: 10px;"></td>
  </tr>
  <tr>
    <td><img src="display_files/angry.png" width="300" style="margin-right: 10px;"></td>
    <td><img src="display_files/angry_emotion.jpg" width="200" style="margin-right: 10px;"></td>
    <td><img src="display_files/angry_grad_cam.jpg" width="200"></td>
  </tr>
</table>

_________________

### To run the program
1) Install python 3.10
2) Install everything you need
   - `git clone https://github.com/rishiswethan/Video-Audio-Face-Emotion-Recognition.git`
   - `cd Video-Audio-Face-Emotion-Recognition`
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
