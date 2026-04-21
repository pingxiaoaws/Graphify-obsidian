---
source_file: "/home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/services/quota.py"
type: "code"
community: "Community 0"
location: "L127"
tags:
  - graphify/code
  - graphify/INFERRED
  - community/Community_0
---

# check_quota()

## Connections
- [[Check if user is within quota      Args         user_email User email address]] - `rationale_for` [EXTRACTED]
- [[QuotaStatus]] - `calls` [EXTRACTED]
- [[generate_user_id()]] - `calls` [INFERRED]
- [[get_monthly_usage()]] - `calls` [EXTRACTED]
- [[get_my_usage()]] - `calls` [INFERRED]
- [[get_quota_status()]] - `calls` [INFERRED]
- [[quota.py_1]] - `contains` [EXTRACTED]
- [[test_quota_check()]] - `calls` [INFERRED]

#graphify/code #graphify/INFERRED #community/Community_0