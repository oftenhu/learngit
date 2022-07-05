The user guild about git

$sudo apt install git	//install and config the  git in local computer.
$git config --global user.name "Wenchao Hu"	
$git config --global user.email "often.hu@163.com"


$mkdir mydirectory	//creat and initialized  a empty repository
$cd mydirectory
$git init


$vim <myfile>		//creat  a file
$git add <myfile>	//to add myfile from  working directory to stage directory.
$git commit -m "append"	//to add myfile from stage to repository.


$git status		//to show the status in working,stage and repository. 
$git diff		//to show the diffrence between working directory and repository.
$git diff HEAD --<file>	//to show the diffrence between working directory adn repssitory in leatest. 
$git log		//to display the change log.
$git reflog		//to show the change log simply.

$git reset --hard HEAD^		//to return the upon modify.
$git reset --hard <commitIP>	//to return the modify with  commitIP.


$git restore <file>	//to discard the changes in working directory.
$git checkout -- <file>	//to discard the chanres in working directory.
$git reset HEAD <file>	//to discard the changes in stage directory.


$git rm <file>		//to delete a file from repository.

Creat a github account
1.sign up with the username(oftenhu)/email(often.hu@163.com)
2.$ssh-keygen -t rsa -C "often.hu@163.com"
3.sign up the GitHub，“Account settings”->“SSH Keys”->"Add SSH Key”，any Title，paste the content of id_rsa.pub file in key.

Creat a new remote repository in github.

Add a local repository to remote.
$ git remote add origin git@github.com:oftenhu/learngit.git   //origin is the name of remote repository.
$ git push -u origin master   //push all of the local repository to remote first(-u). Branch master set up to track remote branch master from origin.
$ git push origin master      //Then, link the branch master of the local repository to remote when the local changed.

Clone the remote repository to local.
1.Creat a new repository named as gitskills in github.
2.$ git clone git@github.com:michaelliao/gitskills.git    //clone remote repository gitskills to local.
3.$ cd gitskills
  $ ls
  README.md
