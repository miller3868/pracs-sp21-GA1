# Repository for my first assignment

Created files and headings using the terminal. Committed those files. 

Changed file wording and format in README file. Added Unix commands and linked text example in COMMANDS file. Staged and committed files again. 

In COMMANDS file, added Git commands under the Git heading, played with formatting of the Unix commands. Staged and committed COMMANDS file. 

Created a directory called Data and created 100 empty dummy txt files with numbers 1-50 and samples A and B for each number. Staged and committed this directory with these files. 

Goal: Rename 100 data files with .txt extension to .csv extension. (This was a challenge for me.) 
- Created git branch called rename-data-files
- Worked on that branch via `git checkout rename-data-files` command

Note: I think I had trouble because I was initially trying to work in the **Data** directory instead of in the **pracs-sp21-GA1** directory with a path specified to **Data**

Used this code loop to rename files:
`for oldname in Data/*.txt  
do
newname=$basename $oldname txt)csv
echo "Old name: $oldname"
echo -e "New name: $newname \n"
git mv "$oldname" "$newname"
done `

Committed renamed files. 

Went back to master branch, merged with rename-data-files branch to incorporate the new file names into the master:

    `git merge rename-data-files -m "Renamed data files from txt to csv"`

Deleted brance **rename-data-files** with code `git branch -d rename-data-files`


