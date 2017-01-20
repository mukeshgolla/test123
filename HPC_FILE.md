1.Setup master node name as <github handler> and compute <githubhandler1> ,< github handler2>.

2.Prepare /etc/hosts file and sync to all nodes.
Cat /etc/hosts and copy output in hosts.md file in github.

3.Prepare local repo for specific server.
Cat /etc/yum.repo.d/local.repo and paste output in local.md file

4.Export /apps folder and /home folder as NFS.
Cat /etc/exports paste in repo.md file

5.In nodes do auto mount NFS exported folders.
Cd to folders and show df -h output in nfs_moun.md

6.Download user_sync file from github tools folder and modify accounding to your master node IP and copy to /usr/sbin  in all nodes.

7.Create a user with git handler name , create password less login to all nodes for this user you need to run user sync in all nodes.
grep git handler name from /etc/passwd copy output to user.md and ssh to <compute node> run date command copy output in password.md

8.Install ganglia using yum , modify the conf file according to document
Access browser in master node http://<master_node_ip>/ganglia  it should show all the nodes , take screen shot and upload ganglia.png

9.Install Pbspro accouding to doc
Paste the pbsnodes command output in pbsnodes.md
qmgr -c “p s” put the output in gmgr.md
login as user then run echo “sleep 60” | grep
run qstat paste the output in qstat.md

10.Install intel compiler in /apps/intel get the licence server from our server.
Paste the out put of which mpiicc in intel.md

11.login as user in cluster and take cpi.c file from git tools folder and compile it using intelmpicc
 #mpirun
mpiexec.hydra -machinefile hostfile np2 ./cpi.c
paste out put in mpi.md

12.Write pbs script for the above.
pbs script output paste in pbs_script.md
