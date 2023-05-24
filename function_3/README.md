For this project, I try four different types of codes. I found BO_UCB_3.ipynb most successful in finding maximum observation. Following are details of the code files in this folder. 
 

## Initial codebase 

BO_UCB_3. ipynb Develop using code from MP-PCMLAI-M12-BayesianOptimNotebook from Required activity 12.2: Jupyter Notebook on Bayesian optimisation. It uses RBF kernel and GaussianProcessRegressor from sklearn.gaussian_process 

Botorch_UCB_3.ipynb  Develop using code from CapstonUsingBotorchNB2.ipynb from week 18 office hours. It uses UpperConfidenceBound from botorch.acquisition 

Monte_carlo_EI_3.ipynb Develop using code from CapstonUsingBotorchNB2.ipynb from week 18 office hours. It uses  qExpectedImprovement from botorch.acquisition.monte_carlo 

BO_EI_3.ipynb Develop using code from https://machinelearningmastery.com/what-is-bayesian-optimization/. It uses estimated improvement using GaussianProcessRegressor from sklearn.gaussian_process and minimize function from scipy 

 

## Code Modifications 

BO_UCB_3.ipynb  
Modify it to work with multiple inputs according to function, limiting the output values between 0 and 1. Modify it to run code in a loop so I can easily experiment with different values of beta, rbf_lengthscale and noise_assumption.  Later modify it to use grid values around the existing highest observed values. 

Botorch_UCB_3.ipynb 
Modify it to work with multiple inputs according to function, limiting the output values between 0 and 1. Modify it to run code in a loop for different values of beta and noise-level, also manually fine-tune different values of num_restarts and raw_samples. It uses UpperConfidenceBound from botorch.acquisition 

Monte_carlo_EI_3.ipynb 
Modify it to work with multiple inputs according to function, limiting the output values between 0 and 1. Modify it to run code in a loop for different values of beta and noise level, also manually fine-tune different values of num_restarts and raw_samples 

BO_EI_3. Ipynb 

Modify it to work with multiple inputs according to function, limiting the output values between 0 and 1. I experiment with different values of noise, length scale, number of iterations etc. It uses estimated improvement using GaussianProcessRegressor from sklearn.gaussian_process and minimize function from scipy.optimize. I tried different values but the output is not useful I produce random values very different or away from existing higher values. 
 
 
## Results 
After fine-tuning the values of beta = 0.001 and noise_level =0.7 in code file BO_UCB_3.ipynb. I am able to push up the observation values from -0.1111 and -0.024 to -0.0044 during the final weeks of the project. With the passage of time, my results are getting better and better if I have more time, I may be able to get the maximum value of this function. Also, I will try look into the other code files again to find out why some functions are working well and some are not. Although in theory, all of them should work. 
 
 
 
