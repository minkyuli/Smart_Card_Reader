# Smart-Card-Reader(SCR)

This is for All Business people.

Most Business people always have name cards.
And They're alwayes preparing to give and take their one's name cards.

In the past, we had to have real things made by paper
But, nowadays, we don't need to that anymore.

we can store name card's infomation easily using AI technology.
Furthermore, we can obtain more information such as context information, location, circumstance, etc

In conclusions, we aim to develop the Smart AI system to collect name cards and to manage name cards 


# Spec

Basic Environment : GCP Vertax AI Workbench

Model : GenerativeModel("gemini-pro-vision") # gemini-2.0-flash is less then gemini-pro-vision in term of multimodel

Benchmarking Model : ollama, qwen

Reference) https://github.com/ella-hong22/smart_card_test


# Performance

In this section, 

We're gonna compare with several models

We conduct model performance test using Gemini, Qwen, llama.

And then we compared the below sequence

1. Create a Set of Correct Answers

2. From Each model's output, we calculate the distance between Correct Answers and Model's Outputs

3. Sort by The high similarity score

4. Rank the Best score and Models

# Results

pd_score.mean()

gemini     0.679097
qwen_3B    0.839706
qwen_7B    0.774510
dtype: float32


# Run

We can run very easily

But, It is possible to run on GCP Vertax AI.

So, you should prepare the environment for that

python Gemini_OCR_model.py

python Gemini_OCR_model_multi_turns.py





