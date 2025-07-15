# AI-Generated Poetry  

This project uses **GPT-2** to generate **AI-powered poetry** based on **user-defined themes**.  
The AI takes a **starting prompt** and creates **a flowing poem** using deep learning.

---

##  Features
 **Installs Required Libraries** – `transformers`, `torch`.  
 **Loads GPT-2 Model** – Uses a **pre-trained GPT-2 text generation model**.  
 **Generates AI Poetry** – Creates **poetic verses** from a given **prompt**.  
 **Displays the AI-Generated Poem** – Prints the **generated poetry in the notebook**.  

---

##  Example Poetry Prompts
Try different themes:
-  `"A lonely moon whispers to the night"`
-  `"The golden sun kisses the morning sea"`
-  `"Love is a river flowing through time"`
-  `"A mysterious forest filled with forgotten dreams"`

---

##  Getting Started

### **Install Dependencies**
- Run the following command:
pip install transformers torch:
- Generate AI Poetry
```python
from transformers import pipeline
Load GPT-2 poetry generator
poetry_generator = pipeline("text-generation", model="gpt2")
def generate_poetry(prompt, max_length=100):
    print(f"Generating poetry for: {prompt}\n")
    poem = poetry_generator(prompt, max_length=max_length, num_return_sequences=1)[0]['generated_text']
    return poem
# Example prompt
prompt = "The golden sun kisses the morning sea"
poetry = generate_poetry(prompt)
print("\n AI-Generated Poetry \n")
print(poetry)
```
---
### Example Output
- Input Prompt
"The golden sun kisses the morning sea": AI-Generated Poem
- The golden sun kisses the morning sea,  
- A dance of light on waves so free.  
- Reflections shimmer, gold and bright,  
- As dawn awakens with tender light.
  
 ### Use Cases
- Creative Writing – AI-assisted poetry composition.
- Inspirational Quotes – Generate poetic phrases and thoughts.
- Storytelling & Lyrics – Experiment with AI-generated literature.

### Future Enhancements
- Custom Poetry Styles – Fine-tune AI to generate haikus, sonnets, and free verse.
- Interactive UI – Deploy a Flask/Streamlit-based poetry generator.
- Thematic Poetry Generation – Enhance AI to write in specific poetic tones.

---

##  Next Steps
- Add **rhyme schemes** (AABB, ABAB, etc.).  
- Fine-tune GPT for **Shakespearean or modern poetry styles**.  
- **Web app version** for real-time poetry generation.

--- 
 MIT License.
