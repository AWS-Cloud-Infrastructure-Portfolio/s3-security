## AWS S3 Access Control & Storage Configuration

Designed and validated Amazon S3 storage configurations with a focus on access control, encryption defaults and configuration visibility. This project demonstrates hands-on ownership of S3 buckets, policy-driven access behavior and lifecycle management using native AWS tooling.

---

## Overview

This project demonstrates the configuration and validation of Amazon S3 buckets from a cloud infrastructure perspective. It focuses on defining access behavior through bucket policies, enabling encryption at rest, validating object access paths and observing how AWS-native tooling surfaces configuration states.

The implementation reflects common responsibilities in Cloud Engineer and Platform Engineer roles, where storage services must be predictable, observable and safely operated.

---

## What I Built

- Multiple S3 buckets representing common real-world access patterns.
- Bucket policies defining private and public access behavior.
- Server-side encryption using SSE-S3 and SSE-KMS.
- Object-level access validation through direct testing.
- Configuration visibility review using AWS Trusted Advisor.
- Complete resource cleanup to ensure cost control.

---

## Diagram

![Lab Architecture Diagram](diagram.png)

---

## Implementation Highlights

- Provisioned private and public S3 buckets to model different access scenarios.
- Applied bucket policies to enforce HTTPS-only access and public read access where required.
- Enabled and compared AWS-managed and KMS-managed encryption options.
- Verified Block Public Access settings for each bucket.
- Validated object accessibility through browser-based testing.
- Reviewed Trusted Advisor output and documented visibility limitations under Free Tier support.
- Removed all buckets, objects and encryption resources after validation.
   
---

## Screenshots

*All screenshots are included in the `screenshots/` folder of this repository.*

---

## Key Takeaways

- S3 access behavior is primarily driven by policy configuration and defaults.
- Encryption should be treated as baseline storage configuration, not an afterthought.
- Misconfigured access paths are best understood through direct validation.
- AWS-native tooling provides useful signals, but engineers must understand its scope and limits.
- Clean teardown is a critical part of responsible cloud infrastructure management.

---

## References

- [AWS S3 Documentation](https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html)
- [AWS S3 Bucket Policies](https://docs.aws.amazon.com/AmazonS3/latest/userguide/example-bucket-policies.html)
- [AWS S3 Server-Side Encryption](https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingServerSideEncryption.html)
- [AWS Trusted Advisor](https://docs.aws.amazon.com/awssupport/latest/user/trusted-advisor.html)

---

## Contact

Maintained by Sebastian Silva C. – Berlin, Germany
LinkedIn: https://www.linkedin.com/in/sebastiansilc
