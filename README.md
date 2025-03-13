# 🚀 API de Cotações de Criptomoedas

Uma API simples para obter cotações de criptomoedas em tempo real, utilizando a CoinGecko API. Retorna preços em **USD** e **BRL**.

## 📌 Funcionalidades
- 🔄 Obtém o preço de qualquer criptomoeda disponível na CoinGecko.
- 💲 Retorna os valores em **dólares (USD)** e **reais (BRL)**.
- ⚡ Rápido e leve, utilizando **Flask**.

---

## 🛠️ Instalação e Execução

### 1️⃣ Clone o repositório
```sh
git clone https://github.com/seuusuario/crypto-api.git
cd crypto-api
```

### 2️⃣ Instale as dependências
```sh
pip install flask requests
```

### 3️⃣ Execute a API
```sh
python app.py
```

A API rodará em **http://127.0.0.1:5000**.

---

## 📡 Como Usar

### 🔍 Obter cotação de uma criptomoeda
```sh
GET /cotacao/{moeda}
```

### 📌 Exemplo de requisição:
```
http://127.0.0.1:5000/cotacao/bitcoin
```

### 📌 Exemplo de resposta:
```json
{
  "moeda": "bitcoin",
  "preco_usd": 69000,
  "preco_brl": 350000
}
```

---

## 🔥 Melhorias Futuras
✅ Suporte a múltiplas moedas em uma única requisição.
✅ Implementação de histórico de preços.
✅ Interface Web para consulta rápida.

---

## 📜 Licença
Este projeto é open-source sob a licença **MIT**. Sinta-se à vontade para contribuir! 🎉

