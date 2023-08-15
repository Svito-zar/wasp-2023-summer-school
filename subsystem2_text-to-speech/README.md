# Text-to-Speech


## Links used during the presentation

### To visualise spectrograms
https://musiclab.chromeexperiments.com/spectrogram/

### The pink trombone
A cool model of the human vocal tract that synthesizes human voice from scratch, controllable with your fingers 

https://dood.al/pinktrombone/



## Instructions to run multispeaker synthesis

### Either install locally using the instructions below or simply use [this colab notebook.](https://colab.research.google.com/drive/12mdEujBj7Wj0b0SaxW83tS-POgifDKBE?usp=sharing)


1. Install miniconda (or any other environment management that you prefer)
```
https://docs.conda.io/en/main/miniconda.htm
```

2. Once installed run
```bash
conda create -n overflow python=3.9
```
3. Install phonemiser and espeak-ng from: 
(This is an additional tool that converts graphemes to phonemes)
```https://bootphon.github.io/phonemizer/install.html ```

Test phonemiser by:

`echo 'hello world' | phonemize`

> Note
> For mac if the above command fails:
>	
```bash
export PHONEMIZER_ESPEAK_LIBRARY=/opt/homebrew/Cellar/espeak/1.48.04_1/lib/libespeak.dylib
```
> or add it it to you .bashrc or .zshrc

4. Install the multispeaker tts system
```bash
pip install git+https://github.com/shivammehta25/OverFlow.git@multispeaker
```
	

5. Additional dependencies in the same environment
```bash
pip install xformers 
pip install triton==2.0.0.dev20221105 --no-deps # (if it fails, its okay move on it is not an absolute necessary)
```

6. Now we can synthesise texts by running this on command line
```bash
overflow --text "<text>"
```
- Change the text prompt by replacing `<text>` with the input text you want to synthesise

### Multiple sentence synthesis per speaker
To synthesise multiple utterances at once, create a text file, break the sentences to one sentence in one line something like this

>inputs.txt
```text
The sun sets over the horizon, painting the sky.
Lost in thought, she wandered through the maze of memories.
A lone tree stands tall in the middle of meadow.
```
Then call:
```bash
overflow --file inputs.txt 
```

### Change speaker
To change the speaker change the `--speaker_id`
```bash
overflow --text "<text>" --speaker_id 23
```
- Replace the speaker id `<23>` to a number between 1-100 to change the speaker default: 49

## Change speaking rate
Play with the flag `--speaking_rate`.
```bash
overflow --file inputs.txt --speaking_rate 0.6
```
- Use a value between between 0 < sr < 1 default: 0.4
- Generally anything between [0.3, 0.6] should get you comprehensible results
