# Repository for git notes

For work with git the firts thing we need to do is to generate a ssh key and register this on our git acount.

We will use the following command lines to this

{Bash}

	# This command will generate the ssh key

	ssh-keygen -t rsa -b 4096 -C "<your email address>"

	# Once we get our key we need to add the SSH key to the SSH agent

	eval "$(ssh-agent -s)"

	ssh-add ~/.ssh/id_rsa

	# Finally we add the test of the id_rsa.pub to our git acount as the instructions of this page https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0105EN-SkillsNetwork/labs/Module2/GitHub_SSHKey.md.html?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-wwwcourseraorg-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDS0105ENSkillsNetwork20083975-2022-01-01

Once we add our SSH key ot out git acount we area ready to start to work with git on local terminal.

For 