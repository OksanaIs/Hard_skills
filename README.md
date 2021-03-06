## Git Branches

1. On the local repository, make branches for:
- Postman
- Jmeter
- CheckLists
- Bug Reports
- SQL
- Charles
- Mobile testing
```
git branch Postman
git branch Jmeter
git branch CheckLists
git branch Bug_Report
git branch SQL
git branch Charles
git branch Mobile_testing
```
2. Push all branches to an external repository:
```
git push origin --all
```
3. In the Bug_Report branch, make a text document with the structure of a Bug report:
``` 
git checkout Bug_Report
touch Bug_report.txt
vim Bug_report.txt
i
Esc
:wq
```
4. Push the Bug_report.txt to an external repository:
```
git add Bug_report.txt
git commit -m "Message"
git push -u origin Bug_Report
```
5. Commit the Bug_Report branch to main:
```
git checkout main
git merge Bug_Report
```
6. Push main to an external repository:
```
git push -u origin main
```
7. In the CheckLists branch, type the structure of the checklist:
```
git checkout CheckList
touch CheckList.txt
vim CheckList.txt
i
Esc
:wq
```
8. Push the structure to an external repository:
```
git add CheckList.txt
git commit -m "Message"
git push -u origin CheckLists
```
9. On the external repository, make a Pull Request of the CheckLists branch in the main:
```
On the GitHub interface:
Compare & Pull request -> Create pull request -> Merge pull request -> Confirm Merge
```
10. Synchronize External and Local Main branches:
```
git pull
```
