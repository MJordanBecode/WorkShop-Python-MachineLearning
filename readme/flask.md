# Installation of Flask

### Apple 
```bash
pip install flask

```
### Ubuntu 
```bash
pip install flask

```
### Window
```bash
pip install flask

```

### __Start a project with Flask__ : 
##### Exemple : 
```bash
from flask import Flask, request, jsonify
from transformers import pipeline

app = Flask(__name__)
chatbot = pipeline('conversational', model='facebook/blenderbot-3B')

@app.route('/chat', methods=['POST'])
def chat():
    user_input = request.json.get('message')
    response = chatbot(user_input)[0]['generated_text']
    return jsonify({'response': response})

if __name__ == '__main__':
    app.run(debug=True)

```
