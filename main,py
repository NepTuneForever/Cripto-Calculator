from flask import Flask, jsonify
import requests

app = Flask(__name__)


@app.route('/cotacao/<moeda>', methods=['GET'])
def get_cotacao(moeda):
    url = f"https://api.coingecko.com/api/v3/simple/price?ids={moeda}&vs_currencies=usd,brl"
    response = requests.get(url)
    
    if response.status_code == 200:
        data = response.json()
        if moeda in data:
            return jsonify({
                "moeda": moeda,
                "dolar": data[moeda]['usd'],
                "reais": data[moeda]['brl']
            })
    return jsonify({"erro": "moeda não encontrada"}), 404

if __name__ == '__main__':
    app.run(debug=True)
