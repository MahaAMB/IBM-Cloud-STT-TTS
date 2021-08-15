# IBM-Cloud-STT-TTS

This task is for the IBM Cloud services speech to text (STT) and text to speech (TTS).

## Speech to Text

- Started by creating a STT service on IBM Cloud.
![Screenshot (432)](https://user-images.githubusercontent.com/53409187/129494330-c8653d79-3af5-4799-9352-f8f6db7acb28.png)

- Using cmd on my PC, I cloned https://github.com/nicknochnack/RealTimeSpeechToText/tree/main/watson-streaming-stt in order to perform the rela-time speech to text.
- Installed pyaudio and websocket-client from the requirements text file by running pip install -r requirements.txt command in cmd.
- Copied the APIKEY and the regione of the STT service in speech.cfg file.
- In the transcribe.py file, I modified the on_message() method in order to open and save the text that has been converted from a recorded real-time audio.

![Screenshot (433)](https://user-images.githubusercontent.com/53409187/129494593-4b43c37e-8d60-414d-8308-18c2d2f165fd.png)

- In cmd, run the ./transcribe.py -t 20 command to start live recording

![Screenshot (363)](https://user-images.githubusercontent.com/53409187/129494668-a8160a65-7765-4dec-bc47-ad665f48772b.png)


## Text to Speech

- Started by creating a TTS service on IBM Cloud.
![Screenshot (434)](https://user-images.githubusercontent.com/53409187/129494754-65f2fce3-6ae1-4fe6-8373-f081a8ea9d51.png)

- Installed ibm_watson and ibm_cloud_sdk_core.
- Copied the APIKEY and the URL of the TTS service and assigned them to declared variables.
- Import the TextToSpeechV1 and IAMAuthenticator in the code.
- The block of code below shows the method to deploy the conversion of text to speech.
![Screenshot (435)](https://user-images.githubusercontent.com/53409187/129494893-5f6bb860-a0f9-45c6-a990-da2e7e179955.png)

- The audio is saved as an mp3 file in the folder of the project.

