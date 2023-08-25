# In this project, we will deploy that expressjs app to AWS, app deployed in an Auto-Scaling Group behind an Application Load Balancer, app will be managed by systemd.

## 1- create launch template for auto scaling group

![crate launch template](./1.png)

### A- give launch template name and description
![set name and description the launch template](./2.png)

### B- add software configuration (os,app server,...)
![choose software for the launch template](./3.png)

### C- Determine the type of instances and the key-pair
![Determine the type of instances and the key-pair](./4.png)

### D- add security group 
![select security group ](./5.png)

### E- under advance details, scroll down, set User data. [click here](https://github.com/Mustafazaareer/book-app-mustafa/blob/master/infrastructure/setup.sh)
![set User data](./7.png)

### F- launch template created .
![view the launch template](./8.png)

## 2-create auto scaling group 
![create auto scaling group](./9.png)

### A- launch template created, and click next.
![set auto scaling group name and set the desired template ](./10.png)

### B- choose all availability zones to make your project more available, and click next.
![set availability zones and subnets](./11.png)

### C- set configurations for load balancer.
![set configurations for load balancer](./12.png)

### D- complete to set configurations for load balancer and choose target group.
![set configurations for load balancer](./13.png)

### E- additional health check configuration, and click next.
![health check configuration](./14.png)

### F- configure group size and scaling policies, and click next.
![configure group size and scaling policies](./15.png)

### G- click next until reach the last page and click create auto scaling group.
![click create auto scaling group](./16.png)

## 3- Wait a while for the commands in the given  init script to be executed.
![target group page](./17.png)

## 4- go to instances to check if the instances was created or not.
![instances page](./18.png)
![show the instance configurations ](./19.png)

## 5- go to terminal and open the instance .
![instance in terminal](./21.png)

## 6- check if app was cloning or not.
![app was cloning](./22.png)

## 7- go to target group page and see if the instance healthy or not.
![if the instance healthy or not](./23.png)

## 8-check if the app work or not.
![app working](./24.png)
![app working](./25.png)


