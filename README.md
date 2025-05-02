from flask import Flask
import random

app = Flask(__name__)

@app.route("/yazitura")
def yazitura():
    sonuc = random.choice(["Yazı", "Tura"])
    return f"Sonuç: {sonuc}"
