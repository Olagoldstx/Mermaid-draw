# Mermaid-draw
Cloud lab
## GuardDuty Security Pipeline

```mermaid
flowchart LR
  GD[Amazon GuardDuty] --> CWE[CloudWatch Events]
  CWE --> KF[Kinesis Firehose]
  KF --> S3[S3 Bucket]
  KF --> ES[Elasticsearch]
  ES --> Kibana[Kibana Dashboard]
  CWE --> SNS[SNS Alerts]
  SNS --> User[Security Team]
