# speech2sing

# Prepare data:
Takes splited songs (vocals and accompaniment) and create dataset from them (split into 2 seconds files of singing and accompaniment pairs).

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OfirShechter/speech2sing/blob/main/data_preparation/Data_Prepare.ipynb)

# Spleeter
Run spleeter on songs in folder to spleet them into vocals and accompaniment.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OfirShechter/speech2sing/blob/main/data_preparation/spleeter.ipynb)

# MelGAN-VC
## MelGAN-VC with power loss
Run MelGAN with power loss factor. <span style="color:red">Original name: Speech2Sing_Ofir.ipynb</span>

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OfirShechter/speech2sing/blob/main/MelGAN-VC/with-power-loss.ipynb)

### results sample:
![Mel Spectrograms](MelGAN-VC\results\with-power-loss\1\mel_spectrograms.png)

<figure>
  <figcaption>Generated Singing:</figcaption>
  <audio controls>
    <source src="MelGAN-VC\results\with-power-loss\1\generated_singing.wav" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</figure>
<figure>
  <figcaption>Generated Speech:</figcaption>
  <audio controls>
    <source src="MelGAN-VC\results\with-power-loss\1\generated_speech.wav" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</figure>
<figure>
  <figcaption>Original Speech:</figcaption>
  <audio controls>
    <source src="MelGAN-VC\results\with-power-loss\1\original_speech.wav" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</figure>
<figure>
  <figcaption>Complete Song Output:</figcaption>
  <audio controls>
    <source src="MelGAN-VC\results\with-power-loss\1\fake_combine.wav" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</figure>

## MelGAN-VC with Identity force and Normalize mel-spectrogram data
<span style="color:red">Original name: Speech2Sing_Ofir_V8_identity_force_lower_acc.ipynb</span>

Normaize both input and generated mel-spectrogram to make sure discriminator have to address all component equally. Add singing as speech output as well, and add identity-loss when the input speech is actually a singing input.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/OfirShechter/speech2sing/blob/main/MelGAN-VC/identity-force-and-normalization.ipynb)

### Singing as input - results sample:
![Mel Spectrograms](MelGAN-VC\results\identity-force-and-normalization\singing\1\mel_spectrograms.png)

<figure>
  <figcaption>Generated Singing:</figcaption>
  <audio controls>
    <source src="MelGAN-VC\results\identity-force-and-normalization\singing\1\generated_singing.wav" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</figure>
<figure>
  <figcaption>Generated Speech:</figcaption>
  <audio controls>
    <source src="MelGAN-VC\results\identity-force-and-normalization\singing\1\generated_speech.wav" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</figure>
<figure>
  <figcaption>Original Speech:</figcaption>
  <audio controls>
    <source src="MelGAN-VC\results\identity-force-and-normalization\singing\1\original_speech.wav" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</figure>
<figure>
  <figcaption>Complete Song Output:</figcaption>
  <audio controls>
    <source src="MelGAN-VC\results\identity-force-and-normalization\singing\1\fake_combine.wav" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>
</figure>

### Speech as input - results sample:

