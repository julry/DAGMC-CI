DAGMC_CI
=========

This contains the files necessary to run Continuous Integration on batlab.org

GIT Repository
_______________

This git repository lives on github.com/svalinn and is owned by the dagmcci group.  

If this git repository is cloned via https you will be unable to push to github.
Instead, this repository should be cloned via ssh (after adding your public ssh key to the git repository). 



Removing CRON jobs from BaTLab
_____________________________
Note:  See the Command Line Tools in the online BaTLab Reference Manual

$ nmi_list_recurring_runs
	-- get the recurring run id of the job you want to kill
	-- should end in .0
$ nmi_rm <recurring run id>
$ nmi_submit recurring_job.run-spec
