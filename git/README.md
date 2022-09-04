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

The firts steo is to clone our git repository we area capable of this using the folllowinf comand

{Bash}

	git clone "ssh direction of repository"

Now that we already clone our repository we can create and modify file on local way. For a saer way of work we can create a branch remotely and then ask for a pull request or actualize the main repository manually. For create and move from workin directory to a branch we can use the following commands:

{Bash}

	# For create a branch use the folllowinf command

	git branch "Name of the branch"

	# To switch between branches.

	git checkout "name of branch"

The manage of files localy don't requiere any special instruction but when we want to update the repository we need to commit and push the file. Also for detect a directory on git we need to create a README.md file inside de directory.

{Bash}

	#This command is used for add a file to directory

	git add "file"

	#This command is used for comment the files we recently generate

	git commit -m "Commit"

	# Finally we push the changes of the file

	git push

The merge of new file could be permomed via github web page or via command line. For command line merge we use the foollowin command

{Bash}

	# Firts we need to be on main command line

	git checkout "name of main command line"

	# Then we merge branches

	git marge "name of secondary branch"