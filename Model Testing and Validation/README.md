## Q1:   How many ways do you know to implement MLOps?  

There are three ways you can go about implementing MLOps:

MLOps level 0 (Manual process): in this level, every step is manual, including data analysis, data preparation, model training, and validation. It requires manual execution of each step and manual transition from one step to another. The assumption is that your data science team manages a few models that don’t change frequently, consequently, there is no Continuous Integration (CI) and Continuous Deployment (CD) and usually, testing the code is part of the notebooks or script execution and the deployment is done in a microservice with REST API.

MLOps level 1 (ML pipeline automation): The goal here is to perform continuous training (CT) of the model by automating the ML pipeline. This way, you achieve continuous delivery of model prediction service. One main characteristic here is we deploy a whole training pipeline, so the model is automatically trained in production, using fresh data based on live pipeline triggers.

MLOps level 2 (CI/CD pipeline automation): is a step further from MLOps level 1. The goal is to get a rapid and reliable update of pipelines in production, and for that, you need a robust automated CI/CD system:
In the CI stage you build source code and run various tests. The outputs of this stage are pipeline components (packages, executables, and artefacts) to be deployed in a later stage.
In the CD stage you deploy the artefacts produced by the CI stage to the target environment. The output of this stage is a deployed pipeline with the new implementation of the model.
However, the data and model analysis step is still a manual process for data scientists before the pipeline starts a new iteration of the experiment.
Source: neptune.ai   
 
## Q2:   What's the difference between Static Deployment and Dynamic Deployment?  
 

In the Static Deployment, the model is trained offline. That is, we train the model exactly once and then use that trained model for a while. The model training is done on the local machine and once the model is complete, it is saved and transferred to the server to make live predictions. The model is packaged into installable application software and then deployed. For example, an application that offers batch-scoring of requests.

In the Dynamic Deployment, the model is trained online. That is, data is continually entering the system and we're incorporating that data into the model through continuous updates, this means that you predict on demand, using a server. The model is then deployed using a web framework like FastAPI or Flask and is offered as an API endpoint that responds to user requests.

Source: developers.google.com   
 
## Q3:   What production Testing methods do you know?  
 

Batch testing: validates the model by performing testing in an environment that is different from its training environment. Batch testing is carried out on a set of samples of data to test model inference using metrics of choice, such as accuracy, RMSE, etc. Batch testing can be done in various types of computes, for example, in the cloud, or on a remote server or a test server. The model is usually served as a serialized file, and the file is loaded as an object and inferred on test data.

A/B testing: It is often used in service design (websites, mobile apps, and so on) and for assessing marketing campaigns. To evaluate the results of A/B testing, statistical techniques are used based on the business or operations to determine which model will perform better in production. A/B testing is usually conducted in this manner:

Real-time or live data is fragmented or split into two sets, Set A and Set B.
Set A data is routed to the old model, and Set B data is routed to the new model.
In order to evaluate whether the new model (model B) performs better than the old model (model A), various statistical techniques can be used to evaluate model performance (for example, accuracy, precision, etc), depending on the business use case or operations.
Then, we use statistical hypothesis testing: The null hypothesis asserts that the new model does not increase the average value of the monitoring business metrics. The alternate hypothesis asserts that the new model improves the average value of the monitoring business metrics.
Ultimately, we evaluate whether the new model drives a significant boost in specific business metrics.
Stage test or shadow test: Before deploying a model for production, the model is tested in a replicated production-like environment (staging environment). This is especially important for testing the robustness of the model and assessing its performance on real-time data. Is done by deploying the develop branch or a model to be tested on a staging server and inferring the same data as the production pipeline. The only shortcoming here will be that end-users will not see the results of the develop branch or business decisions will not be made in the staging server. The results of the staging environment will statistically be evaluated using suitable metrics to determine the robustness and performance of the model.

Source: www.packtpub.com   
 
## Q4:   What's the difference between Batch Processing and Stream Processing?  

Batch and stream processing are two techniques that allow us to have control over the features that we use to generate our real-time predictions.

Batch process features for a given entity at a previous point in time, which are later used for generating real-time predictions.

Here we can perform heavy feature computations offline and have it ready for fast inference.
However, features can become stale since they were predetermined a while ago. This can be a huge disadvantage when your prediction depends on very recent events. (ex. catching fraudulent transactions as quickly as possible).
In Stream Processing the inference is performed on a given set of inputs with near real-time, streaming, features for a given entity.

Here we can generate better predictions by providing real-time, streaming, features to the model.
However, extra infrastructure is needed to maintain data streams (Kafka, Kinesis, etc.) and for stream processing (Apache Flink, Beam, etc.)
Source: madewithml.com   
 
## Q5:   What is Training-Serving Skew?  


Training-serving skew is a difference between performance during training and performance during serving. This skew can be caused by:

A discrepancy between how you handle data in the training and serving pipelines.
A change in the data between when you train and when you serve.
A feedback loop between your model and your algorithm.
The first two bullets above are also known as data drift or covariate shift. The feedback loop problem mentioned in the third bullet point has to be addressed by proper ML system design.

Source: cloud.google.com   
 
## Q6:   What is a Model Registry and what are its benefits?  
 

A Model Registry is a central repository that allows model developers to publish production-ready models for ease of access. With the registry, developers can also work together with other teams and stakeholders, and collaboratively manage the lifecycle of all models in the organization.

A data scientist can push trained models to the model registry. Once in the registry, the models are ready to be tested, validated, and deployed to production in a workflow that is similar to the one below:



This tool bridges the gap between experiment and production activities. This results in a faster rollout of production models. In addition, model registries store trained models for fast and easy retrieval by any integrated application or service. So, software engineers and reviewers can easily identify and select only the best version of the trained models (based on the evaluation metrics), so the model can be tested, reviewed, and released to production.

In addition, the Model registry simplifies model lifecycle management in the following way:

Register, track, and version your trained, deployed, and retired models in a central repository that is organized and searchable.
Store the metadata for your trained models, as well as their runtime dependencies so the deployment process is eased.
Build automated pipelines that make continuous integration, delivery, and training of your production model possible.
Compare models running in production (champion models) to freshly trained models (or challenger models) in the staging environment.
