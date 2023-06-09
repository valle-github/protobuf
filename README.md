# protobuf
Huge thanks to Hussein Nassers Youtube video protobuf.dev/getting-started/pythontutorial/. I*ve used the same steps and to bulid and explain the workflow.

## What is protobuf?
Protobuf is a way to serialize data into a binary format, just 1s & 0s. This means that your data is incomprehensible unless you know the data-structure so you can interpret this into actual data. This enables your data to be way smaller than if it followed any other "readable" data format such as json or csv which is very important when handling larger data volumes.

### How is it done? 
By frist defining the structure of your data (or 'messages' as it's called) in a `.proto`-file. Then using the protoc-executable generate a file in a programming languange of your chosing. Use this file to serialize your data into binary, when read at the other end of some pipeline deserialize the data using the same file again.

## About this repo

This repo contains a jupyter notebook with all code you can execute along with. each step has comments to explain what's going on.
After you've gone though it please edit and play around with it to see that you've grasped the concept.