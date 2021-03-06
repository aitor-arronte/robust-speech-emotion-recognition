# Robust Speech Emotion Recognition
### Speech emotion recognition models and feature extractors

#### Extracting Tonal Rhythm from a directory of speech utterances (audio files)

In order to extract tonal rhythm from utterances, execute the following command:
```
python main.py -a "/the_directory/where_files/are_located/" -e "emotion_tag"
```
Where -a is the directory of the audio files for a given emotion, and -e is the emotion tag.


This command will return the results in a spreadsheet. All closed and maximal patterns will be outputed in 2 different files. Pattern files will be located in the directory "patterns".

To extract unique patterns from a set when compared to another reference set, the following command can be used:
```
python main.py -r 'patterns/neutral_maximal.txt' -c 'patterns/anger_maximal.txt'
```
where -r is the reference file and -c the file with patterns to compare against the reference.

An extra parameter -d can be added to add activation values from an external spreadsheet.

To see all the parameters use the help function -h.

### Graph Neural Network Models for SER

https://github.com/aitor-arronte/gnn-speech-emotion

#### Reference

If you use this software for research please cite the following publication:
```
@inproceedings{alvarez22_speechprosody,
  author={Aitor Arronte Alvarez and Elsayed Issa and Mohammed Alshakhori},
  title={Computational modeling of intonation patterns in Arabic emotional speech},
  year=2022,
  booktitle={Proc. Speech Prosody 2022},
  pages={615--619},
  doi={10.21437/SpeechProsody.2022-125}
}
```
