# Remote backends
* Can be of 2 types - standard/ remote (https://www.terraform.io/docs/backends/types/)
  * Standard - state storage, locking
  * Remote - run operations on a remote machine
* standard backends
  * | Backend  |  Supports Locking? | Encryption  |  Versioning | Authorization | OSS (aka free)? |
    |---|---|---|---|---|---|
    |  artifactory |  No |   |   |   | No  |
    | consul  |  Yes |   |   |   |   |
    |  etcd | No  |   |    | Yes | Yes  |
    |  http | No  |   |    | No  | Yes  |
    |  manta | No  |   |   |   | No  |
    |  S3 | Yes (with DynamoDB)  | Yes (with KMS)  | Yes (Bucket Versioning)  | Yes  | No $$$ |
    |  swift | No  | Yes  |   | Yes  | Yes  |
