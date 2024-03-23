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
1. **Onset (beats)** – ponto de ataque (noteon) de cada evento (nota), em beats. O beat (pulso) é uma unidade usada no arquivo MIDI, semelhante ao pulso musical, porém independente do compasso. Ou seja, a contagem é crescente do início ao fim do arquivo. Noteon e noteoff são instruções MIDI para iniciar e finalizar a execução de um evento (nota).
2. **Duration (beats)** – duração do evento (diferença entre noteon e noteoff) em beats.
3. **MIDI channel** – MIDI channel on which the specific event occurs. Usually, the channel is associated, when using the MIDI protocol, to the choice of instrument or timbre (patch). A different channel carries each timbre. But the composer or researcher can use the channel to separate events according to any other criteria.
4. **MIDI pitch** – the event’s pitch (note), given in the number of semitones, with the central C corresponding to the number 60. MIDI works under the equal temperament system (12 EDO), but once the program renders the matrix, it is possible to work on Parsemat with any other division of the octave.
5. **Velocity** – attack intensity of the event.
6. **Onset (sec)** – Similar to column 1, but with the data measured in seconds.
7. **Duration (sec)** – Similar to column 2, but with the data measured in seconds.

![image](https://github.com/Pauxygnunes/Parsemat/assets/30673056/fb4abb6b-0529-40ab-964b-ecd8cc24fadb)

- To edit the nm table:
1. Click on the cell to be edited.
2. Enter the new value.
- To save the nm table:
1. Click File > Save nm.
2. Alternatively, use the command Shift + S.
3. Select the save location and click OK.
# Control
The Control panel returns information about the MIDI file.
1. The poly and mono buttons indicate the file’s type – monophonic or polyphonic.
2. Clicking the nm button displays the Table panel. The table is editable.
- To edit the nm table:
1. Click on the cell to be edited.
2. Enter the new value.
# Partitioning
Parsemat offers three partitioning options.
1. **Rhythmic** : Rhythmic Partitioning compares attack points and durations between different parts, deducting the partition from each new noteon. This mode is only available for poly files.
2. **Linear**: Linear or Melodic Partitioning matches the melodic configuration of each new height of a melody by deducting partitions that express the development of the melodic texture. This mode is only available for mono files.
3. **Channels**: Channel Partitioning is a flexible mode, which can be used by the composer or researcher in several different applications. For example, in Instrumental Partitioning, where the parts are read by orchestral suits, or in Event Partitioning, where the score is previously prepared by the researcher, assigning different channels to events of a different nature. This mode is only available for poly files.
As the location of pauses affects the formal analysis, there is an option to read noteoffs in the command line version that will be inserted in the following program versions. At the moment, Parsemat, in the standalone version, simply ignores the pauses when creating the partitioning tables.

![image](https://github.com/Pauxygnunes/Parsemat/assets/30673056/ff9fa05d-92c3-4d68-a2ff-2b9f5d034985)

# Graphics
Parsemat offers three chart options:
- **Indexogram** – The indexogram shows the agglomeration and dispersion indices plotted in a mirrored arrangement from a median axis. The upper peaks correspond to maximum variety points (many parts articulating different ideas). The lower peaks correspond to top massiveness points (many parts articulating identical ideas).
- **Partitiogram** – The partitiogram presents the partitions of the piece mapped in phase space. The trajectory outlined by the textural flow of the work offers an overview of the partitions’ repertoire and their relations.
- **Temporal Partitiogram (Parttemp)** – The temporal partitiogram summarizes the indexogram and partitiogram information in an integrated 3D graph. The rotation tool in the Figure window allows rotating the graph, thus having a better understanding of the resulting structure’s topology.

![image](https://github.com/Pauxygnunes/Parsemat/assets/30673056/445d1d70-7767-44c4-9f88-106b668d0844)

- To obtain one of the partitional graphs:
1. Click the corresponding button.
2. A new window opens with the content of the selected graph.
# Exporting
Parsemat also presents some saving and exporting options in the File> Export menu.
- **Export as Tab** – Exports the partition table in Matlab (.m) format. As there are three possible partitions, the program exports the file as tabrit, tablin, and tabchan (corresponding, respectively, to rhythmic, linear, and channel partitioning).
- **Export nm as MIDI** – Exports the note matrix table as a MIDI file. This function is useful when the user made edits directly to the table.
# References
For information on the basic concepts of Particular Analysis, we recommend the following bibliography:
[Partitional Analysis Publications]([url](https://pauxy.net/partitional-analysis-publications/)https://pauxy.net/partitional-analysis-publications/)
# Download and Installation
Parsemat v. 0.9 for Windows
- To install Parsemat v. 0.9 Beta on Windows 64 bits system, download and run the file ParsematWinInstaller_web.exe.
Parsemat v. 0.9 for Mac OS
To install Parsemat v. 0.9 Beta on Mac OS system, download, decompress and run the file ParsematMacInstaller_web.app.zip. After the installation, the program is available through the Launchpad.
# What's new in version 0.9 Beta
1. Version 0.9 – minor adjustments in interface for usability
2. Partition tables can now be saved and loaded, allowing the dialog with the Partops application, which has the same functionality.
3. Note matrix can be saved and loaded.
4. Note matrices export as MIDI files.
5. The table has a structure with editable cells and lines.
6. The rendering of the partitiogram has been revised and has more stability.
7. A new temporal partitiogram (ptemp) summarizes the remaining graphs’ data in a single figure.
8. The figures now show the full Matlab standard figure menu.
9. The title has been removed from the interface and inserted in the title bar.
10. Small adjustments of size, proportion, and color in the window layout.
# About
PARSEMAT – Parseme Toolbox Software Package v. 0.9 Beta. Copyright © 2004-2022 by Pauxy Gentil Nunes Filho.
Developed by Pauxy Gentil Nunes Filho, pauxy.contact@gmail.com
The functions ‘onset’, ‘dur’, and ‘channel’ are part of MIDI Toolbox Software Package, by Tuomas Eerola & Petri Toiviainen, Music Department, ptee@cc.jyu.fi, ptoiviai@cc.jyu.fi, Copyright © 2004, University of Jyvaskyla, Finland.
This program is free software; you can redistribute it and/or modify it under the terms of version 2 of GNU General Public License as published by the FreeSoftware Foundation.
This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. This is free software, and you are welcome to redistribute it under certain conditions. See the GNU General Public License for more details. You should have received a copy of the GNU General Public License along with this program; if not, write to the Free Software Foundation, Inc.,59 Temple Place – Suite 330,Boston, MA 02111-1307, USA.28.




