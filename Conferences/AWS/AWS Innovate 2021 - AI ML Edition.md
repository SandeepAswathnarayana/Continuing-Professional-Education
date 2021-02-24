
## Keynote - Denis V. Batalov, AWS Tech Leader for AI/ML  
- Use cases (Nike, NFL, Envision), Software 2.0, Differential Programming, Machine Intelligence (Knowledge Acquisition + Inference), Types of ML, Typical ML Flow, AWS AI/ML Stack, AWS Panorama use case, Amazon Monitron, Amazon Lookout for Equipment/Vision/Metrics, SageMaker Studio SDE, AGI?, Startups via Amazon with real practical applications (harrison.ai, Onkolyze), Amazon Polly; Brand voice (KFC, National Autralia Bank), REDASA by Imperial College, Amazon Translate - A2I Integration, AWS DeepRacer events (ASU Telemedicine Robot prototype).  

## Prepare your Datasets at Scale using Apache Spark and SageMaker Data Wrangler - Chris Fregly, AWS Senior Advocate, AI/ML  
- Use Apache Spark when using large datasets (Pands, Scikit-learn do not scale to large datasets)  
- Check data quality with AWS Deequ python library and SageMaker Processing Jobs  
- Data Wrangler: Transform 5-star rating to Sentimental (Negative, Neutral, Positive). Steps: (1) Ingest the data using Athena (2) Data types (3) Process numeric (Min-Max Scaler)  
- Bias during Feature Engineering: choose metrics from the options given below.  
- Feature importance: Importance vs Features graph  
- Data Wrangler Feature Store Noteebook  
- Train Apache SparkML models using SageMaker Processing Jobs: Ex - Movie Recommendations  

## Orchestrate and Automate Machine Learning Workflows with SageMaker Pipelines - Antje Barth, AWS Sr Developer Advocate  
- Pretrain -> Feature Engg -> Fine tune - SageMaker pipeline, BERT pipeline, SageMaker Model Registry (to compare the models and deploy), SageMaker Lineage (for artifacts),  
- to be cont...

##  Select the Right ML Instance for your Training and Inference Job - Shashank Prasanna, AWS Senior Advocate, AI/ML  
- Instances for DL training: P3.2xlarge - local mode training and prototyping; P3.x3large - distributed training and multiple experiments; P3.16xlarge - large scale experiements; P3.dn24xlarge - highest performace optimized for distributed training (32GB memory, 100Gbps BW); P4d.24xlarge - 8 GPUs, for SOTA performance.  
- Data access and feeding large datasets to training instances: Moderate and large datasets - Amazon S3 (pipe mode, file mode); Scalable shared file system - Amazon EFS; High-performace file system - FSx.  
- GPU-accelerated training (demo): SageMaker Debugger (CPU/GPU utilization)  
- Haba Gaudi-based instances (of Intel), AWS Trainium  
- His blog post on "Choosing the right GPUs for DL..."  
- Inference Performace: latency, throughput, cost  
- Insances and Accelerators for ML inference: CPU, GPU, Elastic Inference, AWS Inferentia  
- GPU key strength: they are programmable, you can write custom GPU accelerated model using NVIDIA CUDA,  
- Inference Deployment (Demo): by reducing precision you get higher performance  
- What if you can't maximize GPU utilize? - use Amazon Elastic Inference (EI) for variable size GPU acceleration, cost savings  
- Demo: CPU vs Elastic Inference - Throughput is 6x that of CPU  
- Inferentia: custom silicon for ML inference, single-inferentia and multi-inferentia chip instances  
- Demo: operations running on the chip vs operations running on CPU  

## Comparing Models in Production with Multi-Armed Bandits and Reinforcement Learning - Chris Fregly, AWS Senior Advocate, AI/ML  
- A/B tests vs Multi-armed bandit tests: **A/B Tests** - static, cannot add new models after test begins, static traffic split between models A and B, may negatively impact business metrics, must run experiment to completion, no concept of reward for winning model. **Multi-Armed Bandit Tests**: add new model, dynamic shift traffic, explore-exploit strategy, finish experiment early, minimize regret (business impact), maximize reward.  
- Train 2 BERT models with TF & PyTorch: Ex: Sample Review -> Pre-trained BERT model -> Customer Review Classifier.  
- Train a bandit model with RL: code demo,  
- to be cont...



















