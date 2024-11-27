# 🧠 Fine-Tuning DistilBERT with LoRA for Binary Classification  

This project demonstrates how to **fine-tune a DistilBERT model** using **Low-Rank Adaptation (LoRA)** for binary classification tasks. It provides an efficient and lightweight approach to adapt pre-trained language models to new tasks.  

---

## 📂 Notebook Overview  
The notebook [**Fine_tuning_an_LLM_with_LoRA.ipynb**](./Fine_tuning_an_LLM_with_LoRA.ipynb) offers a comprehensive, step-by-step guide to:  
1. Setting up the environment  
2. Loading and preprocessing datasets  
3. Fine-tuning the model using LoRA  
4. Evaluating performance on the test set  

---

## ✨ Key Components  

### **DistilBERT**  
DistilBERT is a smaller, faster, and more efficient version of BERT with **66M parameters**. It retains 97% of BERT’s performance while being:  
- 💡 40% smaller  
- ⚡ 60% faster  

### **LoRA (Low-Rank Adaptation)**  
LoRA is a powerful fine-tuning technique that adds trainable low-rank matrices to the layers of a frozen pre-trained model, significantly reducing the number of parameters required for adaptation.  

---

## 📊 Dataset  

### **IMDB Movie Reviews**  
The dataset consists of **50,000 labeled movie reviews**:  
- 📈 **25,000 reviews for training**  
- 📉 **25,000 reviews for testing**  

Each review is classified as either:  
- Positive 👍  
- Negative 👎  

The IMDB dataset provides a balanced and reliable source for binary classification tasks.  

---

## ⚙️ Data Preprocessing  
1. **Tokenization**  
   - Text is tokenized into numerical representations using the tokenizer from the DistilBERT model.  

2. **Input Features**  
   - The tokenized data is converted into input features like attention masks and token type IDs to feed into the model.  

3. **Label Encoding**  
   - Sentiment labels (positive/negative) are transformed into numerical values for efficient training.  

---

## 🚀 Model Training with LoRA  
Using LoRA, only a small subset of parameters is updated, significantly reducing computational requirements while maintaining high accuracy.  

### Training Steps  
1. Freeze the pre-trained DistilBERT layers.  
2. Add trainable low-rank matrices to specific layers.  
3. Train on the IMDB dataset for binary classification.  

---

## 📈 Performance Evaluation  
- Evaluate the model's performance on the test set using metrics like accuracy, precision, and recall.  
- Analyze the predictions to ensure robustness in sentiment classification.  

---

