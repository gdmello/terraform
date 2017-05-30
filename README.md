# Remote backends
* Can be of 2 types - standard/ remote (https://www.terraform.io/docs/backends/types/)
  * Standard - state storage, locking
  * Remote - run operations on a remote machine
* standard backends
  * | Backend  |  Supports Locking? | Encryption  |  Versioning | Authorization | OSS (aka free)? | Need to Host? |
    |---|---|---|---|---|---|---|
    |  artifactory |  No |   |   |   | No  |  on-prem/ SaaS |
    | consul  |  Yes |   |   |   |   | Yes |
    |  etcd | No  |   |    | Yes | Yes  | Yes |
    |  http | No  |   |    | No  | Yes  | yes | 
    |  manta | No  |   |   |   | No  | SaaS (with CLI) |
    |  S3 | Yes (with DynamoDB)  | Yes (with KMS)  | Yes (Bucket Versioning)  | Yes  | No $ | No |
    |  swift | No  | Yes  |   | Yes  | Yes  | Iaas |
