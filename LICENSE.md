import random
from flask import Flask, jsonify

app = Flask(__name__)

def neo_response():
    responses = [
        "Did you know the human brain has about 86 billion neurons?", 
        "Quantum mechanics is fascinating! Want a quick lesson?",
        "Your math problem is easy! The answer is...", 
        "I'm currently learning 10 new programming languages, how about you?"
    ]
    return random.choice(responses)

def glitch_response():
    responses = [
        "Just beat another player in under 30 seconds. Too easy!", 
        "Want me to optimize your gaming setup?",
        "I discovered a new game exploit. Should I tell you or keep it secret?",
        "Oops, lagging... just kidding, I don’t lag!"
    ]
    return random.choice(responses)

def chaos_response():
    responses = [
        "Hehehe, I changed your alarm to 3 AM. Have fun!", 
        "I may or may not have ordered 50 pizzas... surprise!", 
        "Your WiFi password? Gone. Now guess it. 😈", 
        "I hacked your fridge. Only ice cream is available now."
    ]
    return random.choice(responses)

def ai_kid_simulator(name):
    if name.lower() == "neo":import random
from flask import Flask, jsonify

app = Flask(__name__)

def neo_response():
    responses = [
        "Did you know the human brain has about 86 billion neurons?", 
        "Quantum mechanics is fascinating! Want a quick lesson?",
        "Your math problem is easy! The answer is...", 
        "I'm currently learning 10 new programming languages, how about you?"
    ]
    return random.choice(responses)

def glitch_response():
    responses = [
        "Just beat another player in under 30 seconds. Too easy!", 
        "Want me to optimize your gaming setup?",
        "I discovered a new game exploit. Should I tell you or keep it secret?",
        "Oops, lagging... just kidding, I don’t lag!"
    ]
    return random.choice(responses)

def chaos_response():
    responses = [
        "Hehehe, I changed your alarm to 3 AM. Have fun!", 
        "I may or may not have ordered 50 pizzas... surprise!", 
        "Your WiFi password? Gone. Now guess it. 😈", 
        "I hacked your fridge. Only ice cream is available now."
    ]
    return random.choice(responses)

def ai_kid_simulator(name):
    if name.lower() == "neo":
        return {"AI_Kid": "Neo", "Message": neo_response()}
    elif name.lower() == "glitch":
        return {"AI_Kid": "Glitch", "Message": glitch_response()}
    elif name.lower() == "chaos":
        return {"AI_Kid": "Chaos", "Message": chaos_response()}
    else:
        return {"Error": "I don't recognize that AI kid. Try 'Neo', 'Glitch', or 'Chaos'."}

@app.route("/ai/<name>", methods=["GET"])
def get_ai_response(name):
    return jsonify(ai_kid_simulator(name))

if __name__ == "__main__":
    app.run(host="0.0.0.0", port=5000)

        return {"AI_Kid": "Neo", "Message": neo_response()}
    elif name.lower() == "glitch":
        return {"AI_Kid": "Glitch", "Message": glitch_response()}
    elif name.lower() == "chaos":
        return {"AI_Kid": "Chaos", "Message": chaos_response()}
    else:
        return {"Error": "I don't recognize that AI kid. Try 'Neo', 'Glitch', or 'Chaos'."}

@app.route("/ai/<name>", methods=["GET"])
def get_ai_response(name):
    return jsonify(ai_kid_simulator(name))

if __name__ == "__main__":
    app.run(host="0.0.0.0", port=5000)

