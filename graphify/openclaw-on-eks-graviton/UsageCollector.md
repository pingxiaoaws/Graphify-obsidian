---
source_file: "/home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/services/usage_collector.py"
type: "code"
community: "Community 1"
location: "L76"
tags:
  - graphify/code
  - graphify/EXTRACTED
  - community/Community_1
---

# UsageCollector

## Connections
- [[.__init__()_4]] - `method` [EXTRACTED]
- [[.aggregate_daily()]] - `method` [EXTRACTED]
- [[.aggregate_hourly()]] - `method` [EXTRACTED]
- [[.cleanup_old_events()]] - `method` [EXTRACTED]
- [[.collect_all_instances()]] - `method` [EXTRACTED]
- [[.collect_from_pod()]] - `method` [EXTRACTED]
- [[.run()]] - `method` [EXTRACTED]
- [[.run_collection_cycle()]] - `method` [EXTRACTED]
- [[.stop()]] - `method` [EXTRACTED]
- [[Background service to collect usage data from OpenClaw instances]] - `rationale_for` [EXTRACTED]
- [[Factory function to create Flask application]] - `uses` [INFERRED]
- [[Main Flask application]] - `uses` [INFERRED]
- [[StripProdPrefixMiddleware]] - `uses` [INFERRED]
- [[WSGI Middleware to strip prod prefix before Flask routing]] - `uses` [INFERRED]
- [[create_app()]] - `calls` [INFERRED]
- [[usage_collector.py]] - `contains` [EXTRACTED]

#graphify/code #graphify/EXTRACTED #community/Community_1