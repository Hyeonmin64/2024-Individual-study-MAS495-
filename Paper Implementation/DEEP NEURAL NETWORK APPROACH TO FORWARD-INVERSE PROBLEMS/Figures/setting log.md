Exp 1.1.a :

N_0 = 100
N_b = 16
N_t = 16
N_x = 100
N_obs = 17

N = 10
M = 8

layers = [2, 128, 256, 128, 1]
activation = nn.ReLU()

optimizer = torch.optim.Adam(model.dnn.parameters(), lr = 1e-5)
(no scheduler)

N = 40000  (iteration)

Exp 1.1.b : 

(It took n hour)


