
## Elastic Inference

Amazon Elastic Inference (EI) is a resource you can attach to your Amazon EC2 CPU instances to accelerate your deep learning (DL) inference workloads. Amazon Elastic Inference allows you to attach GPU-powered acceleration to many Amazon machine instances in order to reduce the cost of running deep learning inference (up to 75%). Amazon Elastic Inference supports TensorFlow, Apache MXNet, and ONNX models through MXNet.

Speeds up throughput and decreases latency of real-timeinferences deployed on SageMaker Hosted Services usingonly CPU-based instances but much more cost-effective than afull GPU instance.Must be configured when you create a deployable model andEI is not available for all algorithms yet.