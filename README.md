# CyFuture_Hackathon
This repository contains the data and code files required for building a Legal Contract Reviewer for english contracts using the CUAD dataset.

## Dataset Used

This project leverages a subset of the **Contract Understanding Atticus Dataset (CUAD)** to automate legal contract analysis. CUAD is an expert-annotated dataset designed for **high-precision clause extraction**, featuring:

- **500+ contracts**
- **13,000+ labeled clauses**
- **41 specialized legal categories**

By utilizing CUAD, this system enhances efficiency in **contract review and risk assessment**, helping users quickly identify key provisions.

For more details, visit [CUAD](https://www.atticusprojectai.org/cuad).

## Dataset Conversion for LLaMA Models

Since LLaMA models do not natively support direct ingestion of the CUAD dataset, the data has been **transformed into an optimized format**. The conversion process ensures compatibility and structured input handling for improved legal NLP performance.

- **Converted Dataset:** `alpaca_format_for_llama.json`
- **Conversion Code:** Implemented in `data_conversion.ipynb`
- **Source Dataset:** A subset of the **CUAD (Contract Understanding Atticus Dataset)**, containing **expert-annotated legal contract clauses**.

This adaptation enhances contract clause extraction and facilitates **efficient automated legal review** using large language models.

## 📝 Legal Answering using CUAD + LoRA Fine-tuning(LegalAnsweringUsingCUAD.ipnyb)

This repository contains a Google Colab notebook to **fine-tune a Large Language Model (LLM)** on the [CUAD](https://www.atticusprojectai.org/cuad) dataset for legal contract understanding and question answering. We use **Unsloth** and **LoRA adapters** to efficiently train on long legal texts.

---

## 🚀 Overview of Steps

### 1️⃣ Installation
We install all required libraries including Unsloth.
### 2️⃣ Load and Prepare the Model (Unsloth)
We load a quantized LLaMA-3 model (8B) using Unsloth, with support for long context lengths.
### 3️⃣ Add LoRA Adapters
We apply LoRA adapters so that only a small subset of parameters are updated, reducing memory footprint.
### 4️⃣ Data Preparation
We structure CUAD examples using instruction-style prompts to make them suitable for fine-tuning as described earlier.
### 5️⃣ Train the Model
The model is fine-tuned using the formatted dataset.





# KEY FEATURES


✅ Uses LoRA for memory-efficient fine-tuning

✅ Supports long legal documents with 13,500 token context

✅ 4-bit quantization for low resource usage

✅ Can be run on Google Colab
