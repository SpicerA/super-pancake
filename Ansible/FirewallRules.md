Firewall Rules  

RedTeamFirewall  

| Priority | Port | Protocol | Source | Destination | Notes |  
| :-------- | :---- | :-------- | :------ | :----------- | :----- |  
Inbound:  
| 100      | 22 | TCP | 65.182.253.182 | 10.0.0.7 | Allow SSH from Local Workstation to Jump-Box |  
| 110      | 22 | TCP | 10.0.0.7 | Virtual Network | Allow SSH from Jump-Box to Web Server VMs |  
| 120      | 80 | TCP | 65.182.253.182 | Virtual Network | Allow HTTP access from Local Workstation |  
| 65000    | Any | Any | Virtual Network | Virtual Network | Allow inbound access between Virtual assets |  
| 65001    | Any | Any | AzureLoadBalancer | Any | Allow Load Balancer access to network |  
| 65500    | Any | Any | Any | Any | IMPLICIT DENY all other traffic |  
Outbound:  
| 65000    | Any | Any | Virtual Network | Virtual Network | Allow outbound access between Virtual assets |  
| 65001    | Any | Any | Any | Internet | Allow outbound access to Internet |  
| 65500    | Any | Any | Any | Any | IMPLICIT DENY all other traffic |  

Elk-Stack Firewall

| Priority | Port | Protocol | Source | Destination | Notes |  
| :-------- | :---- | :-------- | :------ | :----------- | :----- |  
Inbound:  
| 100 | 5601 | TCP | 65.182.253.182 | Any | Allow access to Elk-Stack-VM with Kibana |  
| 65000 | Any | Any | Virtual Network | Virtual Network | Allow inbound access between Virtual assets |  
| 65001 | Any | Any | AzureLoadBalancer | Any | Allow Load Balancer access to network |  
| 65500 | Any | Any | Any | Any | IMPLICIT DENY all other traffic |  
Outbound:
| 65000 | Any | Any | Virtual Network | Virtual Network | Allow outbound access between Virtual assets |  
| 65001 | Any | Any | Any | Internet | Allow outbound access to Internet |  
| 65500 | Any | Any | Any | Any | IMPLICIT DENY all other traffic |  
