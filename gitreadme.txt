mkdir mydirectory
cd mydirectory
git init
vim <myfile>
git add <myfile>	/to add myfile to stage directory.
git commit -m "append"	/to add myfile to repository.
git status	/to show the changes
git diff	/to diffrent between working directory and repository.
git log		/to display the change log.
git reset --hard HEAD^		/to return the upon modify.
git reset --hard <commitIP>	/to return the modify with  commitIP.
git reflog	/to show the log simply.
git restore <file>	/to discard the changes in working directory.
git reset HEAD <file>	/to discard the changes in stage directory.
git checkout -- <file>	/to discard the chanres in working directory.
