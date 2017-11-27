This is a notebook tutorial for TensorFlow (mainly thorugh Keras) on MNIST data

You will go through building a simple fully connected (dense - DNN) network, then improve it using convolution (CNN), and then you will explore RNN (LSTM) for the same problem

## Lauunching your AMI 

http://bit.ly/dlami-blog

Windows users can use this bootcamp at: https://github.com/awslabs/aws-ai-bootcamp-labs

Note that there are a few new AMI, choose the one with Conda:

"Deep Learning AMI (Amazon Linux) Version 1.0 - ami-77eb3a0f

Deep Learning AMI with **Conda-based** virtual environments for Apache MXNet, TensorFlow, Caffe2, PyTorch, Theano, CNTK and Keras"

Make sure that you have the **keypair** you are using or download the new one that you created

Connecting to the instance and opening an SSH tunnel for Jupyter:

ssh -i user.pem -L 8888:localhost:8888 ubuntu@ec2-ip-ip-ip-ip.region.compute.amazonaws.com

ssh -i user.pem -L 8888:localhost:8888 ec2-user@ec2-ip-ip-ip-ip.region.compute.amazonaws.com

### TensorBoard 

Opening SSH tunnel for TensorBoard:

ssh -i user.pem -L 6006:localhost:6006 ubuntu@ec2-ip-ip-ip-ip.region.compute.amazonaws.com

ssh -i user.pem -L 6006:localhost:6006 ec2-user@ec2-ip-ip-ip-ip.region.compute.amazonaws.com

tensorboard --logdir=~/TensorFlowTutorials/logs/
