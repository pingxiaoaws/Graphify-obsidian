---
source_file: "/home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/api/proxy.py"
type: "rationale"
community: "Community 4"
location: "L108"
tags:
  - graphify/rationale
  - graphify/EXTRACTED
  - community/Community_4
---

# Proxy to OpenClaw instance root path      This handles the case when accessing /

## Connections
- [[K8sClient]] - `uses` [INFERRED]
- [[proxy_to_instance_root()]] - `rationale_for` [EXTRACTED]

#graphify/rationale #graphify/EXTRACTED #community/Community_4