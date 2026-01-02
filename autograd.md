# Intro to Autograd 

## basic mechanics of a single training pass 
example using a basic RNN
begin with 4 tensors: x the input, h hidden state of the rnn that gives it its memory, and 2 sets of learning weights; one each for the input and the hidden state 

```
x = torch.randn(1,10)
prev_h = torch.randn(1,20)
W_h = torch.randn(202,20)
W_x = torch.randn(20,10)
```