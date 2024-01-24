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

N_0 = 4000
N_t = 20000
N_obs = 40  # 40

parameter_list = [0.1, 0.6, 0.3, 0.9]
(initialization)

optimizer = torch.optim.Adam(model.dnn.parameters(), lr = 1e-4)

scheduler = torch.optim.lr_scheduler.LambdaLR(optimizer=optimizer, lr_lambda=lambda epoch: 0.999 ** epoch, last_epoch=-1, verbose=False)

layers = [1, 64, 64, 2]
activation = sin()

N = 40,000 (iteration)

It 39900: loss = 4.19058961e-05, loss_0 = 2.00872137e-08, loss_r = 4.00767785e-05, loss_obs = 1.80902998e-06
It 39900: alpha = 9.99908447e-01, beta = 4.00222033e-01, delta = 1.00073867e-01, gamma = 3.99845362e-01





