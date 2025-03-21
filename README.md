# Authors

Norberto Casarin (https://github.com/BandoleroNext)
Antonio Gravina (https://github.com/GravAnt)
Gabriele Nanni

# Assignment 1

## Running the code on local machine
To run the code:
1. Install Python 3.12.5 from [here](https://www.python.org/downloads/release/python-3125/).
2. Create a virtual environment (optional)
3. Install the required packages using the following command:
```bash
pip install -r requirements.txt
```
4. Create a directory named `glove_emb` in the `Assignment 1` directory of the project.
5. Download GloVe embeddings from [here](https://nlp.stanford.edu/data/glove.twitter.27B.zip) and extract the file in the `glove_emb` directory.
6. Install CUDA 12.4 from [here](https://developer.nvidia.com/cuda-12-4-0-download-archive). I suggest to download the exe (local) installer type.
7. OPTIONAL: If you want to compute the OOV embeddings by your own (it takes around 40 minutes on my i7 8th gen), uncomment these lines on the notebook:
```python
#OOV_token_to_emb = dict()
#for OOV_token in not_embedded:
#    closest_word, similarity = get_adjusted_embedding(OOV_token, token_to_emb, OOV_token_to_emb)
```
8. Run the notebook.

## Running the code on Google Colab
To run the code on Google Colab, follow these steps:
1. Open the notebook on Google Colab.
2. Upload to the path `/content/drive/MyDrive/` the following files:
    - `test.json`
    - `training.json`
    - `validation.json`
    - `glove.twitter.27B.200d.txt`
    - `OOV_token_to_emb.json`
3. Run the notebook.


# Assignment 2

Note: before running the code, make sure to put the environment variable `HUGGINGFACE_TOKEN` with the value of your Hugging Face token.
