# Placement Assistant using TinyLlama Fine-Tuning with LoRA

## Project Overview

This project demonstrates the fine-tuning of the TinyLlama Large Language Model using the LoRA (Low-Rank Adaptation) technique for creating a Placement Assistant. The assistant is designed to answer placement-related questions covering Data Structures and Algorithms (DSA), Object-Oriented Programming (OOP), Database Management Systems (DBMS), Operating Systems, Computer Networks, Cloud Computing, Git, GitHub, Aptitude, and Interview Preparation.

The objective of this project is to customize a pre-trained language model using a domain-specific dataset and generate meaningful responses to placement-oriented queries.

---

## Objectives

* Fine-tune TinyLlama using LoRA.
* Create a custom Placement Assistant.
* Train the model on placement-related Question-Answer pairs.
* Generate responses for interview and technical preparation questions.
* Demonstrate Parameter Efficient Fine-Tuning (PEFT).

---

## Technologies Used

* Python
* Google Colab
* Hugging Face Transformers
* PEFT (Parameter Efficient Fine-Tuning)
* LoRA (Low-Rank Adaptation)
* Datasets Library
* BitsAndBytes Quantization
* TinyLlama Model

---

## Dataset Description

A custom dataset was created consisting of placement-related Question-Answer pairs.

Topics included:

* Data Structures and Algorithms
* Object-Oriented Programming
* Database Management System
* SQL
* Operating Systems
* Computer Networks
* Cloud Computing
* AWS
* Git and GitHub
* Aptitude Questions
* HR Interview Questions
* Resume Preparation

Example Dataset Entry:

Q: What is GitHub?

A: GitHub is a platform for hosting Git repositories.

Q: What is SQL?

A: SQL is a language used to interact with relational databases.

---

## Methodology

### Step 1: Load TinyLlama Model

The pre-trained TinyLlama model was loaded from Hugging Face.

### Step 2: Prepare Dataset

A custom placement dataset containing Question-Answer pairs was created and converted into Hugging Face Dataset format.

### Step 3: Tokenization

The dataset was tokenized using the TinyLlama tokenizer.

### Step 4: Apply LoRA

LoRA adapters were configured with the following parameters:

* Rank (r): 8
* Alpha: 16
* Dropout: 0.5
* Target Modules:

  * q_proj
  * v_proj

### Step 5: Fine-Tuning

The model was trained using the Hugging Face Trainer API.

Training Configuration:

* Batch Size: 1
* Gradient Accumulation Steps: 4
* Epochs: 5
* Optimizer: AdamW
* Learning Rate: 2e-4

### Step 6: Response Generation

After training, the model was tested with placement-related questions.

---

## Sample Queries

### Query 1

What is GitHub?

Response:

GitHub is a platform for hosting Git repositories and managing software development projects.

### Query 2

What is SQL?

Response:

SQL is a language used to interact with relational databases.

### Query 3

What is AWS?

Response:

AWS stands for Amazon Web Services, a cloud computing platform that provides various cloud services.

---

## Advantages

* Lightweight fine-tuning using LoRA.
* Reduced memory requirements.
* Faster training compared to full model fine-tuning.
* Customizable for domain-specific applications.
* Suitable for educational and placement preparation purposes.

---

## Applications

* Placement Preparation Assistant
* Technical Interview Preparation
* Student Learning Assistant
* Coding Interview Guidance
* Educational Chatbot

---

## Results

The TinyLlama model was successfully fine-tuned on a custom placement dataset using LoRA. The model was able to generate placement-related responses and demonstrate domain adaptation through parameter-efficient fine-tuning.

---

## Future Enhancements

* Increase dataset size to more than 500 Question-Answer pairs.
* Integrate Retrieval-Augmented Generation (RAG).
* Deploy as a web application using Streamlit.
* Add voice interaction capabilities.
* Connect with real-time placement resources.

---

## Conclusion

This project successfully demonstrates the fine-tuning of TinyLlama using LoRA for developing a Placement Assistant. The model learns placement-related concepts from a custom dataset and provides responses to technical and interview-oriented questions. The project highlights the effectiveness of parameter-efficient fine-tuning techniques in creating specialized AI assistants.

---

## Author

Prameesha P

B.Tech Computer Science and Business Systems (CSBS)

Placement Assistant using TinyLlama + LoRA Fine-Tuning

