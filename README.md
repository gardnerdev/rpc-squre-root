
Application which is counting the square root remotely



## Command 
```
python -m grpc_tools.protoc -I. --python_out=. --grpc_python_out=. calculator.proto
```




The following files will be generated:
* calculator pb2.py - containing message classes
    - calculator pb2. Number for request / response variables
* calculator pb2 grpc.py - contains server and client classes
    - calculator pb2 grpc.CalculatorServicer - for the server
    - calculator pb2 grpc.CalculatorStub - for the client


Usage:

1. Activate virtualenv && install packages
2.  Run server:
```
python server.py
```
3. Run client:
```
python client.py
```


```
> python server.py            
Starting server. Listening on port 50051.
INFO:root:Calculating the square root of value: 25.0
```