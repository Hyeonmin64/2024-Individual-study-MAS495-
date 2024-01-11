Exp 1.1.a :

N_0 = 100
N_b = 16 (each side has 16 collocation points, so total number is 32)
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

It 99900: loss = 7.62746026e-07, loss_0 = 1.91584974e-07, loss_b = 1.80624689e-08, loss_r = 3.56225740e-07, loss_obs = 1.96872861e-07, parameter = 3.14168155e-01 

(It took 1 hour 30 minutes)


