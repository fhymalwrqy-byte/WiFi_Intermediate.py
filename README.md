# WiFi_Intermediate.py
 ```python from flask import Flask, request app = Flask(__name__) CORRECT = "1234567890"  @app.route('/verify') def verify():     if request.args.get('username') == CORRECT:         return '{"status":"success"}'     return '{"status":"error"}'  app.run(port=5000) ``` 
server.py
