Asset values for Network Diagram

| Network Name | IP Range |  
| :------------ | :-------- |  
| RedTeamNet | 10.0.0.0/16 |  
| Elk-Stack | 10.1.0.0/16 |  

| Name | Public IP | Private IP | OS Version | Network | Notes |  
| :---- | :--------- | :---------- | :---------- | :------- | :----- |  
| Local Workstation | 65.182.253.182 | | Windows 10 x64 |  
| Jump-Box-Provisioner | 13.66.213.241 | 10.0.0.7 | Ubuntu Linux 18.04 | RedTeamNet | AP to Web Server VMs |  
| Red-Team Load Balancer | 52.250.12.82 | | | RedTeamNet |  
| Web-1 | | 10.0.0.8 | Ubuntu Linux 18.04 | RedTeamNet | DVWA running in Docker container |  
| Web-2 | | 10.0.0.9 | Ubuntu Linux 18.04 | RedTeamNet | DVWA running in Docker container |  
| Web-3 | | 10.0.0.4 | Ubuntu Linux 18.04 | RedTeamNet | DVWA running in Docker container |  
| Elk-Stack-VM | 40.80.156.24 | 10.1.0.4 | Ubuntu Linux 18.04 | Elk-Stack | ELK running in Docker Container |  

* Public IP addresses subject to change
