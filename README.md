# Recommendation-System-for-E-Commerce-Application

Advanced Ensemble Learning • Matrix Factorization • Scalability & Systems Optimization

In this project, I architected and implemented a high-performance recommender system tailored for e-commerce platforms, leveraging a custom ensemble learning framework that combines matrix factorization with bagging techniques to maximize recommendation quality and robustness. The solution tackles key industry-scale challenges in recommender systems — including cold start, data sparsity, scalability, accuracy, computational cost, and diversity of recommendations — through thoughtful algorithmic design and parameter optimization.

At its core, the system learns latent user-item relationships via optimized matrix factorization, while a bagging-inspired ensemble approach aggregates multiple models to reduce variance and improve generalization. I experimented with hyperparameters (e.g., regularization factor, latent feature dimensions, bag size) to drive empirical performance, achieving a test RMSE in the low-tenths percentile on benchmarking data.

The project was developed in GNU Octave, showcasing full procedural control over every phase of the recommendation pipeline, from ratings normalization and matrix construction to prediction aggregation and evaluation. Alongside technical implementation, I documented performance trade-offs and future opportunities for compute efficiency and real-world deployment optimization.

This work exemplifies my ability to design machine learning solutions that balance algorithmic rigor with practical system considerations, and reflects the technical leadership skills required to guide engineering teams in deploying scalable, data-driven products.

1) Platform used: GNU Octave 5.2.0

2) Instructions to run: 
	From the GUI: 
	- Open main.m from the folder.
	- Run the program.
	
	From Command Prompt: 
	- run main.m 

3) Note: The run time may be a bit more due to the ensemble technique I am using. So please wait for the complete execution of the program. The program
generates a valid output. The future scope of this project includes reducing the execution time and also improving the computational efficiency.

4) The program requires the setting of parameters like lambda, features and k. I have experimented with many values and the values set currently in the 
submitted program worked the best for me. The current selection of lambda = 10, features = 30 and k = 8, gives me an RMSE with my test data as good as 0.13%.

Below are some of my observations with different parameter values and their respective RMSE's: 

	a. lambda =  10
	   features =  20
	   k =  5
	   RMSE: 0.50%

	b. lambda =  15
	   features =  20
	   k =  5
	   RMSE: 0.84%

	c. lambda =  10
	   features =  10
	   k =  10
	   RMSE: 1.27%

	d. lambda =  5
	   features =  20
	   k =  10
	   RMSE: 3.68%

	e. lambda =  5
	   features =  10
	   k =  0
	   RMSE: 1.11%

5) References and Resources used: 

	a. https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0184516       
	b. https://paperswithcode.com/paper/on-the-difficulty-of-evaluating-baselines-a             
	c. https://arxiv.org/abs/1901.03888                                                                                            
	d. https://www.coursera.org/learn/machine-learning/lecture/Rhg6r/problem-formulation                                                    
	e. Coursera - Andrew Ng's course for Machine Learning (Recommender System) and its assignment from Week-9.                                                               
	f. https://www.netflixprize.com/assets/GrandPrize2009_BPC_BellKor.pdf
