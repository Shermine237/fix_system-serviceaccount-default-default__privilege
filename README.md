# fix_system-serviceaccount-default-default__privilege
Fix ERROR: Job failed (system failure): prepare environment: setting up credentials: secrets is forbidden: User "system:serviceaccount:default:default" cannot create resource "secrets" in API group "" in the namespace "dev". Check https://docs.gitlab.com/runner/shells/index.html#shell-profile-loading for more information. 

[RUN] kubectl create clusterrolebinding serviceaccounts-cluster-admin \
  --clusterrole=cluster-admin \
  --group=system:serviceaccounts
