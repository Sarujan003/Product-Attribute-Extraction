🧠 LLM Fine-Tuning for Product Attribute Extraction
This project demonstrates how to fine-tune a Large Language Model (LLM) for a Named Entity Recognition (NER) task, specifically targeting product attribute extraction from unstructured text. The fine-tuned model transforms product descriptions into clean, structured flat JSON outputs.


🚀 Key Features
✅ Efficient Fine-Tuning
Uses Unsloth and QLoRA to fine-tune the mistralai/Mistral-7B-Instruct-v0.2 model on consumer-grade GPUs (e.g., Google Colab T4).

🧪 Synthetic Data Generation
Includes scripts to generate and augment datasets with synthetic product descriptions, enhancing robustness and generalization.

🧾 Structured JSON Output
Model trained to return clean, flat key-value pairs in JSON (no nested structures), enabling seamless integration into downstream systems.

🛠 End-to-End Training Pipeline
From data generation to fine-tuning and inference on unseen samples, everything is included in a single notebook.

📥 Input → 📤 Output Example
🔹 Input (Unstructured Description)
Crafted for the Pixel 8 Pro, this sleek champagne gold case is made from carbon fiber. It weighs 2.5 ounces and is produced in Germany.

Output (Flat JSON)
{
  "product": "Pixel 8 Pro",
  "color": "champagne gold",
  "material": "carbon fiber",
  "weight": "2.5 ounces",
  "origin": "Germany"
}
