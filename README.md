
## 1. Create a New User

<br>
<br>


<br>
<br>

![1](https://github.com/user-attachments/assets/47d92d80-d1d6-4b98-be2b-e5414153e3b3)



 <br>
<br>


<br>
<br>


## 2. Editing the Configuration File (slurm.conf)

<br>
<br>


<br>
<br>


![3 1    slurm conf](https://github.com/user-attachments/assets/ace4c580-32de-4772-8f6a-c0e695cd2372)



<br>
<br>


<br>
<br>

![3 2    slurm conf](https://github.com/user-attachments/assets/52bf2610-9d42-4191-8156-c7dfc1742897)

 

<br>
<br>


<br>
<br>

## 3. Navigating and Working with Scripts


 

<br>
<br>


<br>
<br>

![2     scrpt](https://github.com/user-attachments/assets/2322acc7-5ffc-4ad1-b93e-93dfa4c79661)



<br>
<br>


<br>
<br>

##  4. Copy Configuration to System Directories
<br>
<br>


<br>
<br>

![copy slurm cony  to other path](https://github.com/user-attachments/assets/fc8e555e-f07d-403a-8be1-f601a3217885)


<br>
<br>


<br>
<br>
 


## 5. Restarting Slurm Services
  - After editing the configuration, the Slurm services were restarted:
      - systemctl restart slurmd
      - systemctl restart slurmdbd
      - systemctl restart slurmctld

<br>
<br>


<br>
<br>







## 6. Create Account and User in sacctmgr
<br>
<br>


<br>
<br>

![4](https://github.com/user-attachments/assets/06fb1707-a4bb-4b2b-8e4b-5fe6bec1eb02)




<br>
<br>


<br>
<br>


## 7. Create QoS for the User


<br>
<br>


<br>
<br>

![5](https://github.com/user-attachments/assets/c5a754a6-404c-4520-81bf-de3b3b837c99)



<br>
<br>


<br>
<br>






## 8. Modify User Settings (MaxJobs)
<br>
<br>


<br>
<br>


![6](https://github.com/user-attachments/assets/640f8ec5-e8fa-4020-ad25-2be3c3052572)



<br>
<br>


<br>
<br>






## 9. Submitting Jobs as examuser

 

![login to examuser and submit jobs](https://github.com/user-attachments/assets/d5f6d452-ebbc-4e40-a082-1b3154704fef)

<br>
<br>


<br>
<br>


## 10. MaxJobs Exceeded (QoS Limit)
If the user exceeds the MaxJobs limit, the job will be queued with the following message:
squeue

<br>
<br>


<br>
<br>




![final output](https://github.com/user-attachments/assets/5e58d12a-e8b1-49f2-87a2-2820585a7f89)







 <br>
<br>


<br>
<br>






________________________________________


## Key Points:
  ●	User Management: You created a new user, assigned an account, and set job limits.
  
  ●	Configuration Changes: The configuration file (slurm.conf) was edited and copied to the appropriate system directories.
  
  ●	Slurm Services: Restarted necessary Slurm services (slurmd, slurmdbd, slurmctld) after configuration changes.
  
  ●	Job Limits: Managed user job limits through sacctmgr (e.g., MaxJobs=2).
  
  ●	QoS: Created and modified QoS for the user.
  
  ●	Job Submission: Submitted jobs using sbatch and monitored them with squeue.











