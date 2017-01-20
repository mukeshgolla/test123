## Test your self with below  Task.

### FS2 Configuration
---
## NAS 

1. Create NAS Disk 
	- exam
2. Create 2 Shares 
	- support
	- peg
3. Create 2 Users
	- support
	- peg
4. configure the share with below pattren
<center>

|User_Name|support-Permission|Peg-Permission|
| :--------  | :---: | :---: |
| support    | RW    | X   |
| peg        | X     | RW  |

</center>
RW-Read Write

X-no Permission

5. Take below screen shots
	- show all share to exam_share.png
	- show all users to exam_users.png
		
## SAN

1. Create Below Disks
	- BIO Disk of 15GB name ```disk1```
	- BIO Disk of 15GB name ```disk2```
2. access the disk1 in windows client through iSCSI
	- Take the  screenshot of device  manager showing 15GB disk ```exam_iscsi.png```
3. access the disk2 in linux client through iSCSI
	- take the lsscsi output in exam_lsscsi.md

***

### HPC
---
1. Configure the Cluster Show ganglia page and  upload as exam_cluster.png

 	

