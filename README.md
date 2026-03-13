# DrumBeatsVRMidiConvert
Drum Beats VR drag and drop midi file converter

Drag and drop midi file converter for Drum Beats VR
Pretty simple to use, It's a perl script so you need to have perl installed on windows. You also need VLC installed.

# Setup:
You can get perl here http://strawberryperl.com. Just install it and after install open a terminal window and at the command prompt type 'perl' to make sure it's working.

You can get vlc from https://www.videolan.org/vlc/
Running the conversion tool:
Download Convert.zip found here and unzip it

# Step 1: Make sure the path in convert_midi.bat points to your VLC installation path (only need to do this once)
Edit the line in convert_midi.bat that says
set PATH=%PATH%;C:"Program Files (X86)"\VideoLAN\VLC

Make sure this line points to the directory where you installed VLC (for example):
set PATH=%PATH%;C:\VLC

# Step 2: Set up a soundfont file in VLC (only need to do this once)
run VLC and you need to specify a soundfont file
Tools->Preferences->Input Codecs

Click Show All Settings
Input/Codecs->Audio Codec->FluidSynth

Specify a .sf2 soundfont file. I use this one but you can search for different ones to give it a different sound https://musical-artifacts.com/artifacts/874
For certain songs the music will sound better with different soundfont file.

# Step 3: Drag your midi file onto the convert_midi.bat file in windows explorer
Make sure your midi file has a normal name (no spaces, periods, etc)
When generation starts, it will pop open a VLC window. When you see the VLC progress bar has completed, the conversion is done and you may need to manually close the VLC window.

# Step 4: Copy the generated files to the game directory
In the output directory will be your newly created custom song files (song.mid and song.wav)
Put these files in the DrumBeatsVR2\Songs directory or DrumBeatsVR-Beta\DrumBeatsVR\Songs depending on which version you're running.
