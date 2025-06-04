# 🎬 TranscodeX – Serverless Video Transcoding Pipeline

**TranscodeX** is a cloud-native video transcoding pipeline built using AWS services. When a video is uploaded to an input S3 bucket, a Lambda function places a job message in an SQS queue. This message is picked up by an ECS Fargate task running FFmpeg, which transcodes the video and uploads the result to an output S3 bucket. The entire architecture is scalable, event-driven, and provisioned with Terraform.

---

## 🧠 What This Project Demonstrates

- Event-based serverless architecture for video processing
- Use of ECS Fargate for running containerized FFmpeg workloads
- Decoupling with SQS for fault-tolerant, asynchronous execution
- S3 triggers and Lambda f
