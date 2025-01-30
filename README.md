# mlops-identity-verification

# MLOps Identity Verification

This repository contains infrastructure, pipelines, and CI/CD setup for an identity verification system using MLOps best practices. It includes pipelines for inference and retraining for identity verification on aws. 

## 📁 Project Structure
Component	Technology

Drift Detection -> Evidently AI	 -> Lightweight, integrates with Python, and provides interpretable drift metrics.

Compute	-> SageMaker ->	Scalable, managed training/inference, and spot instances for cost efficiency.

Orchestration -> Prefect -> Handles complex workflows (retries, dependencies) and integrates with AWS.

Triggering ->	Lambda + S3	Serverless,  -> event-driven, and cost-effective for sporadic drift checks.

Security ->	IAM Roles  -> Restrict Lambda/Prefect permissions to least privilege (e.g., read S3, invoke flows).