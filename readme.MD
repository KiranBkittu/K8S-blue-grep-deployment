 Blue Green Deployment steps
 
 Step 1:
 blue is origin deployment on 01-blue-deployment.yaml with service 02-main.service.yaml nginx older version

 Plan to upgrade nginx old version to newer version 

 Step 2:
 create same kind of setup with new version of nginx with label name as green 03-green-deployement.yaml with preview service 04-preview-service.yaml to test we require some service so we pointing to preview service fo the green.

 Step 3:
  if everything success in testing of green we shift traffic of 03-green-deployement to 02-main-service.yaml for main service using selectors. after some time we remove blue completly after confirmation of the team.