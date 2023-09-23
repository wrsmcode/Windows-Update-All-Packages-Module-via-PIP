# Windows-Update-All-Packages-Module-via-PIP
here is a simple method, to update ALL Packages, that was installed via PIP. (tested with Python3.X)

1. list all outdated Packages:
2. pip list --outdated
3. Copy the complete list and paste it in here: Test String Field
      https://regex101.com/
4. enter in the Regular Expression field:
/^(\S+)\s*/gm

5. on the right hand, see Match Information - klick on the little icon in the right top field, called Export Matches
6. select on the left plain Text
7. select the omplete Match
8. paste it in Texteditor and save it
9. open cmd in that folder, where you saved the Textfile and enter:
  pip install -r ExportetTextListName.txt -- upgrade

drink a coffee and wait...


It worked fine and updated about 65 Packages, but i get an error:
pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.

some dependencies are conflicted - for me was it 4 packages... - i installed that manually - and it works fine now...

Just an Info to all Windows-Users...

cheers
Joko
   
