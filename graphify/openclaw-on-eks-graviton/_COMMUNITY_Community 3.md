---
type: community
members: 28
---

# Community 3

**Members:** 28 nodes

## Members
- [[Database initialization and connection - PostgreSQL version]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[Delete usage_events older than N days]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[Get a PostgreSQL database connection]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[Get all users with their usage stats (admin only).     Queries usage_events dire]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[Initialize the database with tables]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[Input validation utilities]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/utils/validator.py
- [[Insert a usage event into the database (legacy - used by UsageCollector)]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[Register API endpoint]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/api/register.py
- [[Register a new user      Request Body     {         username johndoe,]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/api/register.py
- [[Validate email address format      Args         email Email address to validat]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/utils/validator.py
- [[Validate password strength      Rules     - At least 8 characters     - Contain]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/api/register.py
- [[Validate username format      Rules     - 3-30 characters     - Alphanumeric, u]] - rationale - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/api/register.py
- [[cleanup_old_usage_events()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[create_user()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[database.py]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[get_all_users_with_usage()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[get_db_connection()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[get_user_by_username()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[init_db()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[init_test_db.py]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/scripts/init_test_db.py
- [[insert_usage_event()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/database.py
- [[main()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/scripts/init_test_db.py
- [[register()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/api/register.py
- [[register.py]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/api/register.py
- [[validate_email()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/utils/validator.py
- [[validate_password()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/api/register.py
- [[validate_username()]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/api/register.py
- [[validator.py]] - code - /home/ec2-user/openclaw-on-eks-graviton/eks-pod-service/app/utils/validator.py

## Live Query (requires Dataview plugin)

```dataview
TABLE source_file, type FROM #community/Community_3
SORT file.name ASC
```

## Connections to other communities
- 5 edges to [[_COMMUNITY_Community 0]]
- 3 edges to [[_COMMUNITY_Community 1]]
- 2 edges to [[_COMMUNITY_Community 9]]
- 2 edges to [[_COMMUNITY_Community 6]]
- 1 edge to [[_COMMUNITY_Community 5]]
- 1 edge to [[_COMMUNITY_Community 2]]

## Top bridge nodes
- [[get_db_connection()]] - degree 11, connects to 2 communities
- [[register()]] - degree 9, connects to 2 communities
- [[main()]] - degree 5, connects to 2 communities
- [[database.py]] - degree 10, connects to 1 community
- [[init_db()]] - degree 5, connects to 1 community