from flask import Flask, render_template

app = Flask(__name__)

@app.route("/")
def home():
    return render_template("index.html")

@app.route("/friend/Varshini")
def friend():
    return render_template("friend.html")

@app.route("/special")
def special():
    return render_template("special.html")

@app.route("/letter")
def letter():
    return render_template("letter.html")

@app.route("/final")
def final():
    return render_template("final.html")

@app.route("/final2")
def final2():
    return render_template("final2.html")


if __name__ == "__main__":
    app.run(debug=True)
