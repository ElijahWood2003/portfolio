# Music Key ML
> #### Date created: December 2024 - Current
>
> ##### Written in: **Python, SwiftUI**
>
> Collaborators: Ivan Fuentes, Carmine Falconi
>
> [Github](https://github.com/ElijahWood2003/audio-key-ml)

A machine learning project I am currently working on with a small group of friends. We are training a ML model on a large data set of music with the goal of teaching it how to continuously find the key-signature being played for live music.

### Creating the Dataset
To create a large dataset with minimal manual labor, I have created a script which takes in a list of text in the format: 
```
[YouTube-music URL], [key-signature] \ENTER
[YouTube-music URL], [key-signature] \ENTER
...
```
Through a series of subscripts, the script outputs this simple input into clean data.
#### Script Output:

1. **Downloads and converts** the Youtube video into a .wav audio file
2. **Stores** the .wav audio file in a local temp directory
3. **Converts** the .wav file into a spectrogram
4. **Stores** the spectrogram in a data directory
5. **Adds the local path** of the spectrogram to a .csv file along with the key-signature
6. **Cleans up** all temporary audio/files created