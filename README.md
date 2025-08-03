# 📝 Markov Chain-Based Text Generator 

This project uses a Markov Chain model to generate poetic phrases inspired by the style of Gulzaar and Prem Chand. The model learns transition probabilities from a dataset of text files and generates new phrases starting from a given seed.

## 📂 Project Structure

```
project/
│
├── files/                # Folder containing input text files
│   ├── story1.txt
│
├── main.py               # Python script for training and generation
├── README.md             # You're reading this file
```

## 🔧 Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/niku-raaz/sent-markov.git
cd sent-markov
```

### 2. Install Required Packages

Make sure you have Python 3 installed. Then install the required libraries:

```bash
pip install numpy pandas nltk
```

And download the necessary NLTK tokenizer:

```python
import nltk
nltk.download('punkt')
```

### 3. Add Your Dataset

Place your `.txt` files containing poetry or prose (preferably in Whitman style) in the `files/` directory. Each file should have the following format:

- Lines of text.
- Use a separator line (`============================`) to indicate the end of a relevant section in a file (optional).

### 4. Run the Program

```bash
python main.py
```

This will output several generated poetic lines using the trained Markov Chain model.



## 🔁 Customization

- **Change the Seed Word**: Modify the `start` parameter in `generate_story()` to explore different results.
- **Adjust Output Length**: Modify `limit` to control the number of tokens generated.
- **Change N-Gram Size**: Pass a different `n_gram` value when calling `make_markov_model()`.

## 📌 Notes

- Works best with poetic or lyrical datasets.
- Results are highly dependent on the dataset quality and size.




