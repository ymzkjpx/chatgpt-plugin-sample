# chatgpt-plugin-sample

Describe your project here.

# Request

@app.post("/todos/<string:username>")
```shell
curl -X POST -H "Content-Type: application/json" -d "{\"todo\":\"$(jot -r 1 1 100) push-ups\!\"}" http://localhost:5002/todos/alice 
```

@app.get("/todos/<string:username>")
```shell
curl  http://localhost:5002/todos/alice
```

@app.delete("/todos/<string:username>")
```shell
curl -X DELETE -H "Content-Type: application/json" -d "{\"todo_idx\":0}"  http://localhost:5002/todos/alice 
```