argocd app patch-resource kong --kind Deployment --resource-name kong-kong --namespace=kong --patch '{"spec":{"template":{"spec":{"env":{"KONG_ADMIN_API_URI":"kong-kong-admin-kong.apps.cwylie-us-west-1b.kni.syseng.devcluster.openshift.com"}}}}}'  --patch-type 'application/merge-patch+json'