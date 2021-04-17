# GRPC EXAMPLE

This is a basic example about that how we use gprc in python. To run this example you should follow commands below.

1. python3 -m venv venv
2. source venv/bin/activate
3. pip3 install -r requirements.txt
4. python -m grpc_tools.protoc -Iprotos --python_out=. --grpc_python_out=. protos/poc_grpc_example.proto 
You will see generated files these poc_grpc_example_pb2.py, poc_grpc_example_pb2_grpc.py 
5. Please open two command line windows. Come to first window and run 
this command to run GRPC server --> python greeter_server.py
6. Please come to second window and run this command to send request to server from client 
--> python greeter_client.py

Note that; if you make some changes in source code then you must run Step 3 to get new build

