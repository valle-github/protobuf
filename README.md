# protobuf
Huge thanks to Hussein Nassers Youtube video https://www.youtube.com/watch?v=46O73On0gyI and Matthias Döring datascienceblog post https://www.datascienceblog.net/post/programming/essential-protobuf-guide-python/

## What is protobuf?
Protobuf is a way to serialize data into a binary format, just 1s & 0s. This means that your data is incomprehensible unless you know the data-structure so you can interpret this into actual data. This enables your data to be way smaller than if it followed any other "readable" data format such as json or csv which is very important when handling larger data volumes.

### How is it done? 
By frist defining the structure of your data (or 'messages' as it's called) in a `.proto`-file. Then using the protoc-executable generate a file in a programming languange of your chosing. Use this file to serialize your data into binary, when read at the other end of some pipeline deserialize the data using the same file again.

## About this repo
This repo contains a jupyter notebook called "main.ipynb" with all code and comments. The comments explain what's going on and you'll understand by executing one cell at a time. Create a venv with the requirements by doing the following commands:

1. ```python -m venv venv```

2. ```source venv/bin/activate```

3. ```pip install -r requirements.txt```

4. ```jupyter notebook```

5. Click main.ipynb in the jupyter interface and you're off to the races!

Bonus assignment: edit the protobuf message utelize more field types andn complexeties, see the protobuf documentation [here](https://protobuf.dev/programming-guides/proto3/)
