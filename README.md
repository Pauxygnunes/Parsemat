# Parsemat
![Parsemat-0 9](https://github.com/Pauxygnunes/Parsemat/assets/30673056/7a7bcee7-2bee-4565-b34c-79fbf10d0900)
Parsemat v. 0.9 Beta is a tool for compositional or analytical tasks of Particular Analysis. 
Analysis. It is a program aimed at composers, researchers in music, mainly texture and form, and those interested in understanding Particular Analysis and its derived theories. Its applications include:

- Formal and textural analysis;
- Identification of copyright traits common to the repertoires of one or more composers;
- Comparison with other types of analysis (harmonic, rhythmic) to deduce structural relationships;
- Analysis of orchestration and distribution of instruments;
- Analysis of melodic structures.

Version 0.9 Beta is in the testing phase, and we offer it as an open-source program.
Overview, instructions, and additional information can be found at https://pauxy.net/parsemat-3/
# Basic Instructions
The Parsemat program interface consists of selection panels (Selection), partitioning (Partitioning), graphics (Graphics) and information about the file (Control), and a panel of tables, where the file data is displayed. The first step is to choose the MIDI file and then select types of analysis and types of graphics to be produced.
# Interface Elements
![image](https://github.com/Pauxygnunes/Parsemat/assets/30673056/35f8eea2-5112-45ca-9625-0e7f1004a8cc)
# Selection
The first step in using the application is selecting a MIDI file.
We recommend that the MIDI file generator program have human performance mechanisms turned off to analyze the musical structure.
To evaluate timbres or categories of events, one must program the different instruments or types in different channels.
Some programs tend to superimpose contiguous notes to create artificial legato or reverb effects; these resources can also affect the analysis.
If the objective is performance analysis, a Non-quantized file may be more suitable.
We recommend preparing the file in advance for the desired results.
- To select the MIDI file to be analyzed:
1. Click on the MIDI button in the Selection panel.
2. Select a MIDI file on your computer.
3. The MIDI file’s name displays on the Selection panel button.
4. The Control panel indicates whether the file is polyphonic or homophonic (we use these terms at that moment in their technical sense, within the MIDI context, meaning whether the file has simultaneous notes or not).
5. The nm – abbreviation for Note Matrix, from the MIDI Toolbox® (Eerola and Toivianien, 2004) will be displayed.
# Note Matrix (nm) Table
The nm or note matrix table presents information about the MIDI file, organized in 7 columns:
1. Onset (beats) – ponto de ataque (noteon) de cada evento (nota), em beats. O beat (pulso) é uma unidade usada no arquivo MIDI, semelhante ao pulso musical, porém independente do compasso. Ou seja, a contagem é crescente do início ao fim do arquivo. Noteon e noteoff são instruções MIDI para iniciar e finalizar a execução de um evento (nota).
2. Duration (beats) – duração do evento (diferença entre noteon e noteoff) em beats.
3. MIDI channel – MIDI channel on which the specific event occurs. Usually, the channel is associated, when using the MIDI protocol, to the choice of instrument or timbre (patch). A different channel carries each timbre. But the composer or researcher can use the channel to separate events according to any other criteria.
4. MIDI pitch – the event’s pitch (note), given in the number of semitones, with the central C corresponding to the number 60. MIDI works under the equal temperament system (12 EDO), but once the program renders the matrix, it is possible to work on Parsemat with any other division of the octave.
5. Velocity – attack intensity of the event.
6. Onset (sec) – Similar to column 1, but with the data measured in seconds.
7. Duration (sec) – Similar to column 2, but with the data measured in seconds.
![image](https://github.com/Pauxygnunes/Parsemat/assets/30673056/fb4abb6b-0529-40ab-964b-ecd8cc24fadb)
- To edit the nm table:
1. Click on the cell to be edited.
2. Enter the new value.
- To save the nm table:
1. Click File> Save nm.
2. Alternatively, use the command Shift + S.
3. Select the save location and click OK.
# Control
The Control panel returns information about the MIDI file.
1. The poly and mono buttons indicate the file’s type – monophonic or polyphonic.
2. Clicking the nm button displays the Table panel. The table is editable.
- To edit the nm table:
1. Click on the cell to be edited.
2. Enter the new value.
