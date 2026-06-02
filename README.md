# TinyLlama LoRA Fine-Tuning

## Deskripsi

Adapter LoRA hasil fine-tuning model TinyLlama-1.1B-Chat-v1.0 menggunakan dataset Databricks Dolly 15K untuk tugas Fine-Tuning Large Language Model (LLM).

## Informasi Model

* Base Model: TinyLlama-1.1B-Chat-v1.0
* Dataset: Databricks Dolly 15K
* Fine-Tuning Method: LoRA (Low-Rank Adaptation)
* Task Type: Causal Language Modeling (CAUSAL_LM)

## Konfigurasi LoRA

* Rank (r): 16
* Alpha: 32
* Dropout: 0.05
* Target Modules:

  * q_proj
  * k_proj
  * v_proj
  * o_proj

## Training Configuration

* Epoch: 3
* Learning Rate: 2e-4
* Batch Size: 2
* Gradient Accumulation Steps: 4
* Hardware: NVIDIA Tesla T4 (15GB VRAM)
* Framework:

  * Transformers
  * PEFT
  * TRL
  * PyTorch

## File Contents

* adapter_config.json : Konfigurasi LoRA
* adapter_model.safetensors : Bobot adapter hasil fine-tuning
* README.md : Dokumentasi model

## Dataset

Databricks Dolly 15K:
https://huggingface.co/datasets/databricks/databricks-dolly-15k

## Author

Kelompok 9

Anggota:

1. Khusnia Fitri - 1203230030
2. Muhammad Fajri Dwi Prasetya Subandi - 1203230076
