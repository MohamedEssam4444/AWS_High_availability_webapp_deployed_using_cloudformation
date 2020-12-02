# AWS_High_availability_webapp_deployed_using_cloudformation
Infrastructure as Code , deploy AWS High availability webapp using cloudformation

## Archeticture : 
![aws infra soln](https://user-images.githubusercontent.com/68178003/100732047-e3087e00-33d4-11eb-82ed-8d2588f47dc1.jpeg)

### steps: 
Run:
* create stack.sh and enter the variables of stack name and parametersfile and templatefile which will be ourinfra.yaml to build infrastructure 
* run update.sh and enter the templatefile variable to be high_availability_webapp.yaml to build autoscaling groups and loadbalancers in order to have a high availability webapp

#### proven steps:

1. app is exposed and accessible through loadbalancer where loadbalacer points to the cluster nodes

![Screenshot from 2020-09-09 13-51-35](https://user-images.githubusercontent.com/68178003/100713622-3e2e7680-33bd-11eb-838c-8232832445df.png)

2. cluster created with shown checks :

![Screenshot from 2020-09-09 14-41-52](https://user-images.githubusercontent.com/68178003/100713631-4090d080-33bd-11eb-8180-f2bafa2b20ec.png)

3. loadbalancer created :

![Screenshot from 2020-09-09 14-42-48](https://user-images.githubusercontent.com/68178003/100713672-4f778300-33bd-11eb-902f-823a9b57a19c.png)

4. loadbalncer listener :

![Screenshot from 2020-09-09 14-43-16](https://user-images.githubusercontent.com/68178003/100713678-530b0a00-33bd-11eb-989b-ff4ebb88b994.png)

5. outputs of cloudformation stacks: 

![Screenshot from 2020-09-09 14-55-19](https://user-images.githubusercontent.com/68178003/100713690-556d6400-33bd-11eb-9da0-cbd3056d1551.png)

6. stack parameters

![Screenshot from 2020-09-09 14-55-54](https://user-images.githubusercontent.com/68178003/100713707-5d2d0880-33bd-11eb-8268-c185e33e50e0.png)
