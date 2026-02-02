# Text Similarity & Embeddings Explorer 🔍
> *A Mini-Project for my CS Class*

## About This Project
Hey! This is a project I built for my Computer Science class to explore how computers understand language. The goal was to build a tool that can look at a sentence and figure out which category it belongs to (like recognizing that "I like apples" is about **Food**).

I used a few different AI models to see how they compare, ranging from older methods like **GloVe** (which is like a dictionary of word vectors) to modern powerhouses like **OpenAI's GPT embeddings** and **Sentence Transformers**.

## What It Does
The app lets you:
1. **Pick Categories**: You define a list of categories (e.g., "Happy", "Sad", "Angry").
2. **Type a Sentence**: You enter any text you want.
3. **Compare**: The app calculates how similar your sentence is to each category using math (Cosine Similarity).
4. **Visualize**: It shows pie charts of the results so you can see which model is the most confident!

## How to Run It
If you want to try this out on your own machine, here is what you need to do:

### 1. Install Requirements
Make sure you have Python installed, then grab the libraries I used:
```bash
pip install -r requirements.txt
```

### 2. Set Up OpenAI (Optional)
If you want to test the OpenAI models (which are really good!), you'll need an API key.
- You can set it in your terminal: `export OPENAI_API_KEY="your-key"`
- OR just type it directly into the app's sidebar when it runs.

### 3. Launch the App
Run this command to start the interface:
```bash
streamlit run miniproject_1_student.py
```

## What I Learned
Working on this was pretty cool because I got to see the difference between "Bag of Words" approaches and actual semantic understanding.

- **GloVe** is fast but sometimes gets confused because it just averages words together. If I say "not happy", it might see "happy" and think it's positive!
- **Transformers & OpenAI** are much smarter. They understand context and word order (like the difference between "Dog bites man" and "Man bites dog").

Feel free to poke around the code if you're curious how it works!
