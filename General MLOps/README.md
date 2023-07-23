# Table of Contents

  1. Why should you learn MLOps?
  2. Interview Question
  3.  Conclusion

## Why Should You Learn MLOps?
Increased efficiency: MLOps allows for the automation and streamlining of ML model development and deployment, which can significantly increase the speed and efficiency of the process.
Improved quality: MLOps provides a framework for testing, monitoring, and maintaining ML models in production, which helps to ensure their quality and performance.
Scalability: MLOps enables organizations to deploy and maintain ML models at scale, which is becoming increasingly important as the use of ML continues to grow.
Better collaboration: MLOps brings together data scientists, engineers, and operations professionals to collaborate and work towards a common goal, improving the overall ML development process.
Better business outcomes: With more efficient, scalable, and high-quality ML models, organizations can drive better business outcomes and gain a competitive advantage.
More job opportunities: With the increasing use of Machine Learning in industry and organizations, there is a high demand for professionals with MLOps skills.
Learning MLOps can help improve ML models’ Development and deployment, ultimately driving better business outcomes and providing more job opportunities.

Thus you must have realized that MLOps is slowly gaining center stage in the field of AI/ML, and in the coming years, it will be one of the must-have skills for every data and ML engineer. So the next time you sir for your first or new job, you can be sure that knowing tit-bits of MLOps will serve an upper hand for you.

Here you will find some of the essential concepts frequently asked in interviews. For your interview preparation, you can go through these directly without going into the depths of the images.


Become a Full Stack Data Scientist
Transform into an expert and significantly impact the world of data science.
## Interview Questions
### Q1. What is the difference between MLOps, ModelOps, and AIOps?
MLOps, ModelOps, and AIOps are all related to machine learning (ML) integration with software development and operations processes, but they have slightly different focus areas.

MLOps (Machine Learning Operations) integrates ML workflows with software development and operations processes. It involves using tools and methodologies to automate and streamline the building, testing, deployment, and monitoring of ML models in production.
ModelOps (Model Operations) is a subset of MLOps that focuses on operationalizing and managing ML models in production. It includes model versioning, monitoring, updating, and managing the models’ lifecycle.
AIOps (Artificial Intelligence Operations) is a broader concept encompassing MLOps and ModelOps and using AI and machine learning in IT operations and IT service management. It involves using AI and machine learning to analyze and make sense of large amounts of data from IT systems and automate tasks such as incident detection and resolution.
### Q2. What is the difference between MLOps and DevOps?
MLOps (Machine Learning Operations) and DevOps (Development Operations) are practices that aim to integrate software development and operations processes, but they have different focus areas.

DevOps is a set of practices aiming to automate and streamline software development and deployment. It involves collaboration between development and operations teams to improve software development and deployment speed, efficiency, and quality.
MLOps, on the other hand, is focused on integrating machine learning (ML) workflows with software development and operations processes. It involves using tools and methodologies to automate and streamline the building, testing, deployment, and monitoring of ML models in production.
MLOps vs DeVops
Source: projectpro.io

### Q3. How do you create Infrastructure in MLOps?
Creating Infrastructure for MLOps involves several steps:

Identify the requirements: Identify the specific requirements for your ML infrastructure, such as storage, computing, and networking needs. This will help you determine the appropriate infrastructure solutions and technologies.
Choose the appropriate cloud provider: Decide on the one that best fits your requirements. Popular choices include Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP).
Create a data pipeline: Create a data pipeline to automate the process of data collection, cleaning, and preparation. This will ensure that your data is ready for model training and deployment.
Set up a version control system: Set up a version control system such as Git to keep track of changes in your code and models. This will help you to roll back to previous versions if necessary.
Create a model training environment: Set up a model training environment using tools such as Jupyter Notebook or Google Colab. This will allow you to train, test and deploy models in a consistent environment.
Automate the model deployment: Automate the model deployment process using tools such as Kubernetes or Docker. This will help you to quickly deploy models to different environments and scale them as needed.
Monitor and maintain the Infrastructure: Regularly monitor and maintain the Infrastructure to ensure that it runs smoothly and quickly to address any issues that arise.
### Q4. How can you create CI/CD pipelines for Machine Learning?
CI is the acronym for Continuous Integration, and CD stands for Continuous Development. It helps automate the software development process. The CI/CD pipeline’s fundamental feature ensures that ML engineers and software developers can create and deploy error-free code as quickly as possible.

CI/CD Pipeline in MLOps
Creating CI/CD (Continuous Integration/Continuous Deployment) pipelines for machine learning (ML) involves several steps:

Set up a version control system: Set up a version control system such as Git to keep track of changes in your code and models. This will help you to roll back to previous versions if necessary.
Automate the model training process: Automate the model training process using tools such as Jenkins or Travis CI. This will allow you to train models regularly and ensure they are up-to-date with the latest data.
Create a testing environment: Set up a testing environment using tools such as py test or unit test to validate the performance of the models after training. This will help to ensure that the models are working as expected.
Automate the model deployment: Automate the model deployment process using tools such as Kubernetes or Docker. This will help you to quickly deploy models to different environments and scale them as needed.
Set up monitoring and logging: Set up monitoring and logging to track the performance of the models in production. This will help you to identify and address any issues that arise quickly.
Create a rollback strategy: Create a rollback strategy in case of issues with the newly deployed model or revert to a previous version.
Test the end-to-end pipeline: Test the end-to-end pipeline by running a complete cycle of Integration, testing, and deployment to ensure that everything is working as expected.
By following these steps, you can create a robust CI/CD pipeline for ML that will train, test, and deploy models consistently and efficiently and help you respond quickly to any issues that arise.

### Q5. What is model or concept drift?
Concept or Model drift is a change in the underlying probability distribution of the input data, which can cause a trained model to become less accurate over time. It mainly occurs when the model performance during the inference phase degrades compared to its version in the training phase. It is also referred to as train /serve skew as the model’s performance is skewed compared to training or serving phases.

## Data and Model drift
The reasons for this could be many:

The underlying data distribution has changed
Unforeseen scenarios might occur- Models trained on pre-Covid-19 pandemic data are likely to perform even worse on data during the COVID-19 pandemic.
The training was conducted in limited categories, but recently there has been a change in the environment, adding another class.
The data contains far more tokens for NLP problems than the training data.
Continuous monitoring of model performance is always necessary to detect model drift. If model performance is persistently poor, the cause should be investigated and appropriate treatment applied. This almost always requires model retraining.

### Q6. How does monitoring differ from logging?
 Monitoring refers to observing the performance of a system to identify issues and trends. In contrast, logging, on the other hand, refers to logging information about a system in a log file. Thus, monitoring has the edge over logging in that it can identify issues that may not be evident in a log file. Also, analyzing the trend helps predict future problems.

### Q7. What testing should be done before deploying an ML model into production?
Different types of testing should be performed before deploying the ML model into production.

Unit testing: To verify that individual components of the model, such as the data preprocessing and feature extraction code, are working as expected
Integration Testing: This tests how different components of a model work together.
Performance Testing: This tests how the model performs under different conditions using metrics like accuracy, precision, recall, and F1-score on a held-out test dataset.
A/B testing: Compare the model’s performance against a baseline model or a previous version of the model.
Stress testing: Evaluate the model’s performance under extreme conditions, such as handling large amounts of data or dealing with edge cases.
User acceptance testing: Get feedback from real users to ensure that the model meets their needs and provides accurate results.
Security and Privacy testing: Evaluate the model’s security and privacy features, such as data encryption, authentication, and access control, to ensure that sensitive data is protected.
### Q8. What is the A/B split approach of model evaluation?
A/B split is a model evaluation method where two groups of data, group A and group B, are randomly selected from a larger dataset. One group (group A) is used to train the model, while the other group (group B) is used to test the model’s performance. This approach allows a more accurate assessment of the model’s performance because it is tested on unseen data. Additionally, randomly splitting the data helps to avoid any potential biases that may be present in the data.


### Q9. What is the importance of using version control for MLOps?
Version control is essential for MLOps because it enables tracking and managing codes and changes to codes and data. It helps maintain the reproducibility of data and keeps track of what has been tried in the past. Additionally, it helps prevent data loss and makes collaborations on projects more accessible.

### Q10. What is the difference between A/B testing model deployment and Multi-Arm Bandit?
A/B testing and Multi-Arm Bandit (MAB) are both methods of model deployment that involve comparing multiple versions of a model. However, they are used for different purposes and have some key differences.

A/B testing compares two or more model versions to determine which performs better. It is typically used to optimize a specific metric, such as conversion or click-through rate. In A/B testing, the different versions of the model are deployed to a fixed percentage of users, and the performance of each version is evaluated over a fixed period.

Multi-Arm Bandit (MAB) is an online experimentation method that adapts to the performance of different model versions as they are deployed. It is used to balance the trade-off between exploration (trying different versions of the model to find the best one) and exploitation (using the best-performing version of the model to maximize a specific metric). The MAB algorithm uses a strategy that assigns different probabilities to different model versions to decide which one to deploy next. It then adjusts the probabilities based on the results of previous deployments.

### Q11. What is the difference between Canary and Blue-Green strategies of deployment?
Canary and blue-green deployment are strategies used to deploy new versions of a software application without disrupting the existing service. However, they work in slightly different ways.

Canary deployment is a technique where a new version of the application is deployed to a small subset of users or servers. This allows the new version of the application to be tested in a real-world environment, with real users, before it is deployed to the entire user base. Any issues with the new version of the application will be identified and resolved before the new version is deployed to the entire user base.

On the other hand, blue-green deployment involves maintaining two identical environments, one for the current version of the application (blue) and one for the new version (green). The new version is deployed to the green environment when a new application is ready. This new version is then tested to ensure it is working as expected. Once it is confirmed that the new version is working correctly, the traffic is redirected to the green environment, and the blue environment is taken offline.

### Q12. Why would you monitor feature attribution rather than feature distribution?
Monitoring feature attribution rather than feature distribution can be beneficial in certain situations because it provides more information about how the model’s specific features contribute to its overall performance.

Feature attribution refers to determining the importance or contribution of each feature in a model’s output. It can be used to identify which features are most important in making a prediction and how much each feature contributes to the final decision. This information can help understand the model’s behavior, identify potential issues or biases, and decide how to improve the model.

On the other hand, feature distribution refers to the distribution of values for a specific feature across the dataset. While it is helpful to understand the distribution of features in the data, monitoring feature distribution alone may not provide enough information about how the model uses those features to make predictions.

Thus, monitoring feature attribution rather than feature distribution can be helpful because it provides more information about how specific features of the model are contributing to its overall performance, which can help understand the model’s behavior, identify potential issues or biases, and make decisions about how to improve the model.

### Q13. What are the ways of packaging ML Models?
There are different ways to package a machine learning model for deployment, including creating a standalone executable, using containers, deploying on a serverless architecture, using cloud-based services, and creating APIs for the model.

Standalone Executable: A standalone executable is a self-contained package that includes the ML model and its dependencies. This can be deployed on various platforms and does not require any additional software to be installed.
Containers: Containers are a way to package and deploy software applications, including ML models. They allow for a consistent runtime environment and make it easy to deploy the model in different environments. Popular containerization technologies include Docker and Kubernetes.
Serverless: Serverless deployment is a way to run code without having to provision or manage servers. ML models can be deployed as a function-as-a-service (FaaS) and triggered by specific events. This allows for cost-efficient deployment and scaling.
Cloud-based: Cloud providers such as Amazon Web Services (AWS), Google Cloud Platform (GCP), and Microsoft Azure offer various services for deploying ML models. These services include pre-built containers, serverless options, and cloud-based ML platforms.
APIs: ML models can be exposed as an API (Application Programming Interface) that allows other applications to request the model and receive predictions as a response. This can be implemented using a web framework such as Flask or Django.

Source: dataaiku.com

### Q14. What is the concept of “Immutable Infrastructure”?
Immutable Infrastructure refers to the fact that your Infrastructure should be treated as immutable or unchangeable. That means that once you have deployed your Infrastructure, you should not attempt to change it. And if a change is needed, you should deploy a new version of the Infrastructure. This strategy helps prevent concept drift and maintains the Infrastructure efficiently.

### Q15. Mention some common issues involved in ML model deployment.
Below are some common issues that need to be taken care of in deploying ML models.

Making sure the model is executable in production
Managing model versions and dependencies
Automating model training and deployment
Monitoring model performance in production
Dealing with data drift

### Q16. What Do You Mean By MLOps?
The topic of operationalizing ML models is the focus of MLOps, also known as Machine Learning Operations, a developing field within the more major AI/DS/ML arena.

The main goal of the software engineering approach and culture known as MLOps is to integrate the creation of machine learning/data science models and their subsequent operationalization (Ops).

Conventional DevOps and MLOps share certain similarities, however, MLOps also differs greatly from traditional DevOps.

MLOps adds a new layer of complexity by focusing on data, whereas DevOps primarily focuses on operationalizing code and software releases that cannot be stateful.

The combination of ML, Data, and Ops is what gives MLOps its common name (machine learning, data engineering, and DevOps).

### Q17. How Do Data Scientists, Data Engineers, And ML Engineers Vary From One Another?
It varies, in my opinion, depending on the firm. The environment for the transportation and transformation of data, as well as its storage, is built up by data engineers.

Data scientists are experts in utilizing scientific and statistical techniques to analyze data and draw conclusions, including making predictions about future behavior based on the trends that are now in place.

Software engineers were studying operations and managing deployment infrastructure a few years ago. Ops teams, on the other hand, were studying development while using infrastructure as a code. A DevOps position was produced by these two streams.

MLOps is in the same category as Data Scientist and Data Engineer. Data engineers are gaining knowledge about the infrastructure needed to support model lifecycles and create pipelines for ongoing training.

Data scientists seek to develop their model deployment and scoring capabilities.

A production-grade data pipeline is built by ML engineers utilizing the infrastructure that transforms raw data into the input needed by a data science model, hosts and runs the model, and outputs a scored dataset to downstream systems.

Both data engineers and data scientists are capable of becoming ML engineers.

### Q18. What Distinguishes MLOps From ModelOps And AIOps?
When constructing end-to-end machine learning algorithms, MLOps is a DevOps application that includes data collection, data pre-processing, model creation, model deployment in production, model monitoring in production, and model periodic upgrade.

The use of DevOps in handling the whole implementation of any algorithms, such as Rule-Based Models, is known as ModelOps.

AIOps is leveraging DevOps principles to create AI apps from scratch.

### Q19. Can You Tell Me Some Of The Benefits Of MLOps?
Data scientists and MLOps developers can quickly rerun trials to ensure that models are trained and assessed appropriately since MLOps helps automate all or most of the tasks/steps in the MDLC (model development lifecycle). Additionally permits data and model versioning.
Putting MLOps ideas into practice enables Data Engineers and Data Scientists to have unrestricted access to cultivated and curated datasets, which exponentially accelerates the development of models.
Data scientists will be able to fall back on the model that performed better if the current iteration does not live up to expectations thanks to the ability to have models and datasets versioned, which will significantly enhance the model audit trail.
As MLOps methods strongly rely on DevOps, they also incorporate a number of CI/CD concepts, which enhances the quality and dependability of the code.

### Q20. Can You Tell Me The Components Of MLOps?
Design: MLOps heavily include design thinking. Starting with the nature of the issue, testing hypotheses, architecture, and deployment

Model building: Model testing and validation are part of this step, along with the data engineering pipelines and experimentation to set up the best machine learning systems.

Operations: The model must be implemented as part of the operations and continually checked and evaluated. The CI/CD processes are then monitored and started using an orchestration tool.

### Q21. What Risks Come With Using Data Science?
It is difficult to scale the model across the company.
Without warning, the model shuts down and stops functioning.
Mostly, the accuracy of the models gets worse with time.
The model makes inaccurate predictions based on a specific observation that cannot be further examined.
Data scientists should also maintain models, but they are pricey.
MLOps can be used to reduce these risks.

### Q22. Can You Explain, What Is Model Drift?
When a model’s inference phase performance (using real-world data) deteriorates from its training phase performance, this is known as model drift, also known as idea drift (using historical, labeled data).

The model’s performance is skewed in comparison to the training and serving phases, hence the name “train/serve skew.”

Numerous factors, including:

The fundamental way that data are distributed has altered.
The training focused on a small number of categories, however, an environmental shift that just took place added another area.
In NLP difficulties, the real-world data has a disproportionately larger amount of number tokens than the training data.
Unexpected occurrences, such as a model built on pre-COVID data being predicted to perform significantly worse on data collected during the COVID-19 epidemic.
Continuously monitoring the model’s performance is always required to identify model drift.

Model retraining is nearly always required as a remedy when there is a persistent decline in model performance; the reason for the decline must be identified and appropriate treatment procedures must be used.

### Q23. How Many Different Ways May MLOps Be Applied, In Your Opinion?
There are three methods for putting MLOps into practice:

MLOps level 0 (Manual Process): In this level, all steps—including data preparation, analysis, and training—are performed manually. Each stage must be carried out manually, as well as the transition from one to the next.

The underlying premise is that your data science team only manages a small number of models that aren’t updated frequently.

As a result, there isn’t Continuous Integration (CI) or Continuous Deployment (CD), and testing the code is typically integrated into script execution or notebook execution, with deployment taking place in a microservice with a REST API.

MLOps level 1 (automation of the ML pipeline): By automating the ML process, the objective is to continuously train the model (CT). You can accomplish continuous model prediction service delivery in this way.

Our deployment of a whole training pipeline ensures that the model is automatically trained in production utilizing new data based on active pipeline triggers.

MLOps level 2 (automation of the CI/CD pipeline): It goes one step above MLOps level. A strong automated CI/CD system is required if you want to update pipelines in production quickly and reliably:

You create source code and execute numerous tests throughout the CI stage. Packages, executables, and artifacts are the stage’s outputs, which will be deployed at a later time.
The artifacts created by the CI stage are deployed to the target environment during the CD step. A deployed pipeline with the revised model implementation is the stage’s output.
Before the pipeline begins a new iteration of the experiment, data scientists must still do the data and model analysis phase manually.

### Q24. What Separates Static Deployment From Dynamic Deployment?
The model is trained offline for Static Deployment. In other words, we train the model precisely once and then utilize it for a time. After the model has been trained locally, it is stored and sent to the server to be used to produce real-time predictions.

The model is then distributed as installable application software. a program that allows for batch scoring of requests, as an illustration.

The model is trained online for Dynamic Deployment. That is, new data is constantly being added to the system, and the model is updated continuously to account for it.

As a result, you can make predictions using a server on demand. After that, the model is put into use by being supplied as an API endpoint that reacts to user queries, using a web framework like Flask or FastAPI.

### Q25. What Production Testing Techniques Are You Aware Of?
Batch testing: By conducting testing in a setting different from that of its training environment, it verifies the model. Using metrics of choice, such as accuracy, RMSE, etc., batch testing is done on a group of data samples to verify model inference.

Batch testing can be carried out on a variety of computing platforms, such as a test server, a remote server, or the cloud. Typically, the model is provided as a serialized file, which is loaded as an object and inferred from test data.

A/B testing: It is frequently used for analyzing marketing campaigns as well as for the design of services (websites, mobile applications, etc.).

Based on the company or operations, statistical approaches are used to analyze the results of A/B testing to decide which model will perform better in production. Usually, A/B testing is done in the following way:

Live or real-time data is divided or segmented into two sets, Set A and Set B.
Set A data is sent to the outdated model, while Set B data is sent to the updated model.
Depending on the business use case or processes, several statistical approaches can be used to evaluate model performance (for example, accuracy, precision, etc.) to determine whether the new model (model B) outperforms the old model (model A).
We then do statistical hypothesis testing: The null hypothesis says that the new model has no effect on the average value of the business indicators being monitored. According to the alternative hypothesis, the new model increases the average value of the monitoring business indicators.
Finally, we assess if the new model results in a significant improvement in certain business KPIs.
A shadow or stage test: A model is evaluated in a duplicate of a production environment before being used in production (staging environment).

This is crucial for determining the model’s performance with real-time data and validating the model’s resilience. is carried out by inferring the same data as the production pipeline and delivering the developed branch or a model to be tested on a staging server.

The sole drawback is that no business choices will be made on the staging server or visible to end users as a result of the development branch.

The resilience and performance of the model will be assessed statistically using the results of the staging environment using the appropriate metrics.

### Q26. What Distinguishes Stream Processing From Batch Processing?
We can manipulate the characteristics that we utilize to produce our real-time forecasts using two processing methods: batch and stream.

Batch process features from a prior point in time for a specific object, which is then utilized to generate real-time predictions.

Here, we are able to do intensive feature calculations offline and have the data prepared for quick inference.
Features, however, an age since they were predetermined in the past. This might be a major drawback if your prognosis is based on recent occurrences. (For instance, identifying fraudulent transactions as soon as feasible.)
With near real-time, streaming features for a specific entity, the inference is carried out in stream processing on a given set of inputs.

Here, by giving the model real-time, streaming features, we can get more accurate predictions.
However, additional infrastructure is required for stream processing and to maintain data streams (Kafka, Kinesis, etc). (Apache Flink, Beam, etc.)

### Q27. What Do You Mean By Training Serving Skew?
The disparity between performance when serving and performance during training is known as the training-serving skew. This skew can be induced by the following factors:

A difference in how you handle data between the pipelines for serving and training.
A shift in the data from your training to your service.
A feedback channel between your algorithm and model.

### Q28. What Do You Mean By Model Registry?
Model Registry is a central repository where model creators can publish models that are suitable for use in production.

Developers can collaborate with other teams and stakeholders to manage the lifespan of all models inside the business using the registry. The trained models can be uploaded to the model registry by a data scientist.

The models are prepared for testing, validation, and deployment to production once they are in the register. Additionally, trained models are stored in model registries for quick access by any integrated application or service.

In order to test, evaluate, and deploy the model to production, software developers and reviewers can quickly recognize and choose just the best version of the trained models (based on the evaluation criteria).

### Q29. Can You Elaborate On The Benefits Of Model Registry?
The following are some ways that model registry streamlines model lifecycle management:

To make deployment easier, save the runtime requirements and metadata for your trained models.
Your trained, deployed, and retired models should be registered, tracked, and versioned in a centralized, searchable repository.
Create automated pipelines that enable continuous delivery, training, and integration of your production model.
Compare newly trained models (or challenger models) in the staging environment to models that are currently operating in production (champion models).

### Q30. Can You Explain The Champion-Challenger Technique Works?
It is possible to test various operational decisions in production using a Champion Challenger technique. You have probably heard about A/B testing in the context of marketing.

For instance, you might write two distinct subject lines and distribute them at random to your target demographic in order to maximize the open rate for an email campaign.

The system logs an email’s performance (i.e., email open action) in relation to its subject line, allowing you to compare each subject line’s open rate to determine which is the most effective.

Champion-Challenger is comparable to A/B testing in this regard. You can use decision logic to evaluate each outcome and select the most effective one as you experiment with various methods to come to a choice.

The most successful model correlates to the champion. The first challenger and the matching list of challengers are now all that is present in the first execution phase instead of the champion.

The champion is chosen by the system for further job step executions.

The challengers are contrasted with one another. The new champion is then determined by the challenger who produces the greatest results. 

The tasks involved in the champion-challenger comparison process are listed below in more detail:

Evaluating each of the rival models.
Assessing the final scores.
Comparing the evaluation outcomes to establish the victorious challenger.
Adding the fresh champion to the archive
### Q31. Describe The Enterprise-Level Applications Of The MLOps Lifecycle?
We need to stop considering machine learning as only an iterative experiment in order for machine learning models to enter production. MLOps is the union of software engineering with machine learning.

The finished result should be imagined as such. Therefore, the code for a technological product has to be tested, functional, and modular.

MLOps has a lifespan that is comparable to a conventional machine learning flow, with the exception that the model is kept in the process until production.

The MLOps Engineers then keep an eye on this to make sure the model quality in production is what is intended. 

Here are some use-cases for several of the MLOps technologies:

Model Registries: It is what it appears to be. Larger teams store and maintain track of version models in model registries. Even going back to a previous version is an option.
Feature Store: When dealing with bigger data sets, there could be distinct versions of the analytical datasets and subsets for specific tasks. A feature store is a cutting-edge, tasteful way to use data preparation work from earlier runs or from other teams as well.
Stores for Metadata: It is crucial to monitor metadata correctly throughout production if unstructured data, such as picture and text data, are to be used successfully.

## Conclusion
If you have been able to answer all the questions, then bravo! If not, there is nothing to be disheartened about. The real value of this blog is to understand these questions and to be able to generalize them when faced with similar questions in your next ML Interview! If you struggled with these questions, do not worry! Now is the time to sit down and prepare these concepts.


### Your key takeaways from this article would be:

A concrete understanding of MLOps, ModelOps, and AIOps and how they differ from DevOps.
How to create infrastructure and the CI/CD pipelines in MLOps
The concept of model drift
The different tests that need to be performed before deploying an ML model in the production pipeline
The difference between A/B testing and Multi-Arm Bandit methods of model deployment
The importance of version control in MLOp and different methods of packing ML Models
The concept of Immutable Infrastructure and some of the common issues incurred during ML Model Deployment
If you go through these thoroughly, I can ensure that you have covered the length and breadth of MLOps. The next time you face similar questions, you can confidently answer them! I hope you found this blog helpful and that I successfully added value to your knowledge. Good luck with your interview preparation process and your future endeavors!
