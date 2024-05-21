# TransformerTTS - Neural Speech Synthesis with Transformer Network

## Overview

This project implements the neural speech synthesis model described in the paper "Neural Speech Synthesis with Transformer Network" by Naihan Li et al. The implementation uses PyTorch and leverages the multi-head attention mechanism of the Transformer architecture to improve training efficiency and address long-range dependency issues inherent in RNN-based models like Tacotron2.

<div>
<img src="https://drive.google.com/uc?export=view&id=1JYfBLWSj0vCSz_uVniMuIYOW8T49oSGV" width="800"/>
</div>

## Features

- **End-to-End TTS**: Directly converts phoneme sequences to mel spectrograms.
- **Transformer Architecture**: Utilizes self-attention for parallelization and better handling of long-term dependencies.
- **Enhanced Training Efficiency**: Approximately 4.25 times faster training compared to Tacotron2.
- **High-Quality Output**: Achieves a MOS score of 4.39, close to human speech quality.

## Installation

### Prerequisites

- Python 3.7+
- NumPy
- matplotlib
- SpeechBrain

### Setup

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/transformer-tts.git
   cd transformer-tts
   ```
2. Download and extract the dataset: https://data.keithito.com/data/speech/LJSpeech-1.1.tar.bz2
3. Run the training script in the notebook

## Usage

### Preprocessing
The preprocessing is handled by SpeechBrain.



### Training

Train the Transformer TTS model using the preprocessed data

### Inference
TODO

## Configuration

Following SpeechBrain's conventions, the YAML file is used to set all the configurable parameters for the model, training, and inference processes. Key parameters include:

- **Model Parameters**: Number of layers, number of heads, embedding dimensions, etc.
- **Training Parameters**: Batch size, learning rate, number of epochs, etc.
- **Data Parameters**: Paths to training data, validation data, and test data.

## References

- [Neural Speech Synthesis with Transformer Network](https://arxiv.org/abs/1809.08895)
- [Tacotron2: Natural TTS Synthesis by Conditioning WaveNet on Mel Spectrogram Predictions](https://arxiv.org/abs/1712.05884)
- [Attention Is All You Need](https://arxiv.org/abs/1706.03762)
- [WaveNet: A Generative Model for Raw Audio](https://arxiv.org/abs/1609.03499)

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

This README provides a comprehensive guide to setting up, training, and evaluating a neural speech synthesis model using Transformer networks in PyTorch. For any issues or questions, please open an issue on the project's GitHub repository.

#### My Pretrained Model
1. If you want to load from my latest checkpoint, download the zipped file from here: https://drive.google.com/file/d/18HjNB_W6dfqv8UOv32USlYTjBG2mTelT/view?usp=drive_link
2. Extract the files using this "tar -xvf file.tar.gz"
3. Run the files containing the code
4. Run the training script
