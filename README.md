# CloudEngineStudy
Alt_School_LiveClassSession
Creating or Adding a new SHH key on Github. This is to authenticate my machine


1.	first generate an SSH Key.
In the Linux VM, run the following command
ssh-keygen -t ed25519 -C ediaadada@gmail.com
enter a passphrase. 
An SHA key is generated in a pic like output

2.	copy the key.
cat ~/.ssh/id_ed25519.pub
ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAINj19BjizMywhZoJX0IkWoMiatSnvXNHQcaG+Lq8kk2+ ediaadada@gmail.com


3.	Add the key to Github
Go to Github SSH setting
Click Add new 
Then paste the generated SSH or SHA key. You can name it. I named this vagrant VM


4.	Test the connection
ssh -T git@github.com
It should ask you a few questions and also have you confirm passphrase created earlier then a welcome message with you usefrname should appear on the screen


5.	You can the clone a repo from your github
git clone git@github.com:username/repo-name.git
git clone git@github.com/adada-e/reponame.git
