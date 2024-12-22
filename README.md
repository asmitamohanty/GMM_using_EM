# Algorithmic Comparison of GMM & K-Means with Manual EM Implementation
### Comparing KMeans &amp; GMM using EM Insights

This project explores Gaussian Mixture Models (GMM) with a focus on manual implementation using Expectation-Maximization (EM) algorithm. The key goal of this project is to develop & analyze GMM clustering method with EM, followed by comparing the results with KMeans clustering. The implementation is done manually, emphasizing the probabilistic approach of GMMs. K-Means clustering is used to initialize the GMM by providing initial cluster labels, membership probabilities & other GMM parameters like mean, covariances & mixing weights. The project highlights the iterative nature of the EM algorithm and compares the clustering results of GMM with K-Means. 

This was part of a graded MS coursework associated with the course: EE541 - A Computational Introduction in Deep Learning, taken at University of Southern California (USC). 

### Why Manual GMM with EM?
To understand the mathematical algorithm of GMM & EM & customizing the initialization or convergence criteria, debug & analysis of every step, providing granular control & enabling detailed comparison with KMeans 

#### Objective
- Implement GMM by manually applying EM algorithm.
- Compare clustering results of GMM vs KMeans with visualization
- Analyze the evolution of cluster assignments

#### Project Workflow
- KMeans Clustering: For initialization of GMM parameters & visualization
- GMM Initialization: KMeans labels to initialize membership probabilities (converted to one-hot-encoded), also initialize GMM parameters (means, covariance, weights)
- EM Algorithm: Explicitly derives E (Expectation) & M (Maximization) steps. Iterate over EM steps, updating the GMM parameters & probabilities
- Visualize & Analyze Results: Plotting cluster plots from EM iterations & compare with KMeans, study the evolution of EM plots

#### Results
- The evolution of clusters at every EM step demonstrates variation of the cluster size
- Datapoints keep adjusting themselves due to change in their cluster assignments every EM iteration, resulting in change in the cluster centroid positions
-  Better performance than KMeans due to soft clustering as a result of membership probabilities rather than hard clustering from KMeans

#### Limitations
- Poor initialization from KMeans can result in GMM converging to suboptimal solutions or slow convergence, leading to worse performance. Need robust initialization techniques to combat this.

#### Key Files
- **notebook** : Jupyter notebook with the complete code & results
- **data** : A simple ordered pair dataset with 3 cluster labels: Head, Left Ear, Right Ear. Total samples: 490

  
