# My CKA Exam experience
In this post I'm sharing my exam experience and the resources I used to prepare for it.

The exam gives you 3 hours to complete 24 questions. Actually you have to complete 24 tasks on 6 Kubernetes clusters.
I took the exam on the 1st of December and the clusters were running the 1.11.1 version of Kubernetes.

First of approaching the exam always check the Curriculum Overview and the Candidate Handbook from the following page to see if there is any update https://www.cncf.io/certification/cka/.

You should not expect any questions around beta features. If the exam is running on Kubernetes 1.11.1 than you should not expect questions on features that are in beta for that version of Kubernetes.

All the clusters are systemd based and this means that you will never use kubeadm in any case. Actually kubeadm is not in beta anymore and they could decide to update the exam with it.

## Exam Preparation:

Here is the list of material I used to approach the exam:

1. KTHW on premises : https://blog.csnet.me/2018/04/on-prem-k8s-thw/. There is the same version for Azure, GCP and AWS but just repeat this tutorial as many time as possible. This will make you comfortable with certificates, systemd services and troubleshooting every single component. In th exam you need to be comfortable with systemd (create the systemd service for kubelet, journalctl to get the logs, fix the services and so on...)

2. Go through this list: https://github.com/walidshaari/Kubernetes-Certified-Administrator. It will give you all the theoretical concepts around Kubernetes primitives and some really good tips on troubleshooting the cluster components.

3. The internet is full of free courses to start Kubernetes from 0. I mean if you want to start from 0 knowledge here is the entire updated list of materials you can use: https://docs.google.com/spreadsheets/d/10NltoF_6y3mBwUzQ4bcQLQfCE1BWSgUDcJXy-Qp2JEU/edit#gid=0

4. During the exam you can have 1 open tab to browse the entire Kubernetes.io domain. During my study time I used to create bookmarks on my browser tab for every single page that I found useful. For example I bookmarked every single page containing yaml template that I found useful to be reused (affinity, daemonsets, volumes and so on...). You can copy and paste from that pages or directly curl the yaml link in the exam. Next you can edit it with vim and apply -f it ;)

5. The 
