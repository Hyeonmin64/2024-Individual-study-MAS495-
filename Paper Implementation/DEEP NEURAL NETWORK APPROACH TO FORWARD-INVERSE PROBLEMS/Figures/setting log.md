Exp 1.1.a :

N_0 = 100
N_b = 16 (each side has 16 collocation points, so total number is 32)
N_t = 16
N_x = 100
(N_res = 16*99 = 1584)

N = 10
M = 8 
(N_obs = 10*7 = 70)

layers = [2, 128, 256, 128, 1]
activation = nn.ReLU()

optimizer = torch.optim.Adam(model.dnn.parameters(), lr = 1e-5)
(no scheduler)

N = 40,000  (iteration)

Exp 1.1.b : 

N_0 = 200
N_b = 40
N_t = 40
N_x = 100
(N_res = 40*99 = 3960)


N = 40
M = 25
(N_obs = 40*24 = 960)

layers = [2, 20, 20, 20, 20, 20, 20, 20, 20, 1]
activation = nn.Tanh()

optimizer = torch.optim.Adam(model.dnn.parameters(), lr = 1e-5)
(no scheduler)

N = 100,000 (iteration)
It 99900: loss = 7.62746026e-07, loss_0 = 1.91584974e-07, loss_b = 1.80624689e-08, loss_r = 3.56225740e-07, loss_obs = 1.96872861e-07, parameter = 3.14168155e-01 

(It took 1 hour 30 minutes)

=========

Exp 1.2 : 

N_0 = 200
N_b = 40
N_t = 40
N_x = 100
(N_res = 40*99 = 3960)


N = 40
M = 25
(N_obs = 40*24 = 960)

layers = [2, 20, 20, 20, 20, 20, 20, 20, 20, 1]
activation = nn.Tanh()

optimizer = torch.optim.Adam(model.dnn.parameters(), lr = 1e-5)
(no scheduler)

N = 100,000 (iteration)
It 99900: loss = 7.62746026e-07, loss_0 = 1.91584974e-07, loss_b = 1.80624689e-08, loss_r = 3.56225740e-07, loss_obs = 1.96872861e-07, parameter = 3.14168155e-01 

(It took 1 hour 30 minutes)



