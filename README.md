# PUBG AutoMontage Maker

Inputs a directory containing shadowplay clips, combines them all in time stamped order into one movie file output.


# Usage
* Install ffmpeg
* Install pip3 requirements

`python3 pubg_automontage.py --input_dir $DIR_CONTAINING_MP4_FILES --output_dir $OUTDIR`

This repository also contains a dockerfile in case you don't want to system install anything. Run with:

`docker run -it --rm -v ~/Desktop/vids:/usr/io murtis/pubg_automontage`
