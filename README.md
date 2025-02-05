# **Machine Translation System (Transformer-based)**
### **By: Omer Chaudhry**

## **Overview**
This project implements a **neural machine translation model** using the **Transformer encoder-decoder architecture**. The system translates **German sentences into English** using a **custom-built Transformer model** trained on the **Multi30k dataset**.  

The project follows a step-by-step approach:
1. **Implement the Transformer architecture** from scratch.
2. **Develop decoding algorithms** including **greedy decoding** and **beam search**.
3. **Evaluate translations** using **BLEU score**.
4. **Visualize attention maps** to understand how the model aligns words between languages.

---

## **Key Features**
✔ **End-to-End Machine Translation** – Uses a Transformer model to translate German to English.  
✔ **Custom-built Transformer** – Implemented manually, without relying on prebuilt libraries like Hugging Face.  
✔ **Greedy and Beam Search Decoding** – Compares different decoding strategies for translation.  
✔ **BLEU Score Evaluation** – Measures translation accuracy against ground truth references.  
✔ **Attention Visualization** – Shows how the model focuses on different words in the source sentence.

---

## **Technologies Used**
- **Python 3.x**
- **PyTorch** – Deep learning framework.
- **TorchText** – Data processing and tokenization.
- **NumPy** – Numerical computing.
- **Matplotlib** – Visualization (for attention maps).
- **NLTK** – BLEU score evaluation.

---

## **Installation and Setup**
### **1. Install Required Dependencies**
Run the following commands to install necessary packages:
```bash
pip install torch==2.3.0 torchtext==0.18.0
pip install numpy matplotlib spacy
python -m spacy download en_core_web_sm
python -m spacy download de_core_news_sm
```

### **2. Clone the Repository**
```bash
git clone https://github.com/your-repo/machine-translation.git
cd machine-translation
```

### **3. Run the Jupyter Notebook**
Start Jupyter Notebook and open the **main.ipynb** file:
```bash
jupyter notebook main.ipynb
```

---

## **Usage**
1. **Train the Model:** Run all the cells in `main.ipynb` to train the Transformer model on the **Multi30k dataset**.
2. **Translate a Sentence:** Use the provided `translate()` function to generate English translations from German input.
3. **Evaluate Performance:** The model's accuracy can be assessed using the **BLEU metric**.
4. **Visualize Attention:** The `analyze_sentence()` function generates heatmaps showing how the model attends to different words.

---

## **Expected Outputs**
- **Translation Example:**
  ```
  German Input: "Drei Kinder essen Eis, während ein Elternteil zuschaut"
  Model Output: "Three kids eat ice cream while a parent watches"
  ```
- **BLEU Score Evaluation:**
  ```
  Student BLEU Score: 28.4
  NLTK BLEU Score: 28.3
  ```
- **Attention Heatmap:**  
  Displays how the model aligns words between the source and target languages.

---

## **Future Improvements**
🔹 **Train on a larger dataset** to improve fluency.  
🔹 **Implement Transformer variants** (e.g., BERT or GPT-based translation).  
🔹 **Optimize beam search** for better translation quality.  
🔹 **Fine-tune hyperparameters** for improved accuracy.  

---

## **Contributors**
- **Omer Chaudhry**
- **Professor Ellie Pavlick (Brown University)**
