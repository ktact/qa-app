# git clone後の環境構築
```bash
npm install
```

# アプリ実行
```bash
# from the qa-app/backend directory
node src
```

# 動作確認
```bash
# issue an HTTP GET request
curl localhost:8081

# issue a POST request
curl -X POST -H 'Content-Type: application/json' -d '{
  "title": "How do I make a sandwich?",
  "description": "I am trying very hard, but I do not know how to make a delicious sandwich. Can someone help me?"
}' localhost:8081

curl -X POST -H 'Content-Type: application/json' -d '{
  "title": "What is React?",
  "description": "I have been hearing a lot about React. What is it?"
}' localhost:8081

# re-issue the GET request
curl localhost:8081
```
