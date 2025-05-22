@@ -1,65 +1,81 @@
📚 Knowledge Graph Construction From Text:

# 📚Knowledge Graph Construction From Text:

This project extracts subject–predicate–object triplets from user-input sentences and visualizes them as a knowledge graph.

✨ Features
-> Extracts triplets like (subject, relation, object) from English text.

-> Supports multiple user inputs.
## ✨Features

- Extracts triplets like (subject, relation, object) from English text.

- Supports multiple user inputs.
- Visualizes knowledge graphs using NetworkX and matplotlib.
-  Handles basic passive and active voice constructs.

-> Visualizes knowledge graphs using NetworkX and matplotlib.

-> Handles basic passive and active voice constructs.

📁 Project Structure:
Knowledge-Graph-Construction/
## 📁 Project Structure
```bash
 Knowledge-Graph-Construction/
├── main.py                # Main program to run the input loop and visualize graph
├── src/
│   ├── extractor.py       # spaCy-based triplet extraction logic
│   └── graph_builder.py   # Graph construction and aesthetic visualization
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation
```
## 🚀 Installation

🚀 Getting Started:
1. Clone the Repository:
1. Clone the Repository

```bash
git clone https://github.com/AmreenShaheen/Knowledge-Graph-Construction.git
cd knowledge-graph-construction

```
2. Install Dependencies

```bash
Create a virtual environment (optional but recommended):
python -m venv venv
source venv/bin/activate  # on Windows use: venv\Scripts\activate

3. Install the required packages:
```
3. Install the required packages
```bash
pip install -r requirements.txt

4. Download the spaCy language model:
```
4. Download the spaCy language model
```bash
python -m spacy download en_core_web_sm
```

💻 Usage:
python main.py

    
## 💻 Usage/Examples

```
python main.py
```
You will be prompted to enter multiple sentences or paragraphs. Type exit to stop and visualize the knowledge graph.

Example Input:
```
Elon Musk founded SpaceX.

```
Expected Triplets:
```
('Musk', 'found', 'SpaceX.')

📊 Output
A static but a visual graph window will open.
```

Nodes represent entities (subjects/objects).

Arrows represent the relationships (predicates).

Labels are clean and color-coded for clarity.

📌 Future Improvements
Enable interactive web-based graphs using tools like pyvis or D3.js.
## 📊 Output
- A static but a visual graph window will open.

Integrate co-reference resolution for better pronoun handling.
- Nodes represent entities (subjects/objects).

Extend extraction with deep NLP (transformers, OpenIE, etc.).
- Arrows represent the relationships (predicates).

🧑‍💻 Author
Amreen Shaheen A
- Labels are clean and color-coded for clarity.
