from flask import Flask, request, jsonify

app = Flask(__name__)

@app.route('/run', methods=['GET'])
def run_task():
    task = request.args.get('task')
    # Implement your task execution logic here
    return jsonify({"message": f"Task {task} is being executed"}), 200

@app.route('/read', methods=['GET'])
def read_path():
    path = request.args.get('path')
    # Implement your path reading logic here
    return jsonify({"message": f"Reading path: {path}"}), 200

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=8000)
