### http://www.git-scm.com/book/en/v2/Git-Branching-Branching-Workflows 

git init

echo "asdfasdf">README.MD

git add README.MD		

Nimmt Datei ins 'commit'-index (staging-area) auf, nach bearbeitung wiederholen



git status

git diff	#zeigt änderungen der letzten Bearbeitung 

git diff --stage	#zeigt diese zur letzten 'commit'


git commit 	#erzeugt commit -v for noted changes

git commit -m "Story 182: Fix benchmarks for speed" #for fast command line access

git commit -a -m "Story 182: Fix benchmarks for speed" # erledigen



git rm --cached   #löscht deteien aus der staging-area, aber nicht lokal (--cached)

git rm log/\*.log #escape with \ -- deletes all *.log files (also local)

git reset   	#setzt staging-area zurück

git reset HEAD CONTRIBUTING.md	#nimmt datei aus staging-area in tracked-area


git mv asd.1 asd.2 #verschiebt dateien UND aktulaisiert den commit-index

git log --graph		#zeigt das log mit branch-graph

git log --pretty=format:"%h - %an, %ar : %s" --since="2 years 1 day 3 minutes ago"

git log --pretty="%h - %s" --author=getarun --since="2008-10-01" --before="2008-11-01" --no-merges


git remote add https://github.com/paulboone/ticgit

git pull		# holt dateien aus allen remotes und merged in working-files

git fetch	#holt deteien, aber merged nichts

git clone	#holt dateien (bennnt diesen origin) und merged diese in die lokale  master branch

git remote show origin




git push origin master	#schreibt änderungen auf den server

git tag v3.5  	#tag für den commit (screenshot)

git push v3.5	#



git branch testing	#erzeugt einen neuen branch

git checkout testing	#wechselt nach testing

vim README.MD	#irgendeine änderung

git commit -a -m 'changes done are ...'
