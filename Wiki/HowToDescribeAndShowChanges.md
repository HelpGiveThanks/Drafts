###Overview/Outline of Movie How to Describe and Show Changes to HelpGiveThanks Solution Files on GitHub
Version 1, Copyright 2014 by David Matson. Creative Commons Attribution-ShareAlike 3.0

*15 Seconds*  

What you need to improve solutions, describe, and commit improvements to GitHub: 

* FileMaker 10 or above 
* Chrome
* Clone of HelpGiveThanks GitHub Solution Repositories (click the 'clone in desktop' button on GitHub to get these)
* TextMate for Mac or Notepad++ for Windows, 
* GitHub for Mac or Windows 
* GitHub user account

*1 minute*  
####A. Create a Specific Action Log entry describing basic improvements to screens/layouts, buttons, and scripts.   
 Create a description of your changes in the Specific Action Log.  Doing this helps you not only keep track of changes as you work toward fixing some problem or adding a new feature, but creating a Specific Action entry also allows you to track your time toward this fix/feature.
 
 Note in [brackets] any layout objects affected by changes.
 Include object's Help # and screen/window name between the brackets: [window/screen name #].
 Go to Help to look up any screen/window object's number.  Window/screen names are at the top of each window/screen.
 
 *5 minutes, 10 seconds* 
 
####B. Commit script changes to GitHub 
**Create PDF of FileMaker script**  

1. Select a script in FileMaker.  
2. From the file menu select print.  
3. In the print dialogue box choose to save the script as a PDF.  
4. Save or replace (don't change the name) the  file on the Desktop or other place where you can easily remember to delete these PDF files when finished with the commit process.

   *6 minutes, 30 seconds*  

   **Update script file in GitHub Mac/Windows Folder**  
5. Open PDF in Chrome or if Chrome is already open showing a previous FileMaker PDF file then just refresh Chrome, and any replaced file of the same name will now show up in Chrome.  
6. Select All and copy text.  
7. Open GitHub TextMate or Notepad++ file for the copied script.  
8. Select All and paste copied Chrome PDF text into open script file. 

   *9 minutes*    

   NOTE: In rare cases where a hyphen ends up at the end of a line of text, the paste will not work due to this known issue in Chrome: https://code.google.com/p/chromium/issues/detail?id=327349&can=1&q=copy%  To fix this problem, just add some spaces in the script before the hyphen, so in the PDF it moves to another line.
 
   *11 minutes, 30 seconds*  

   **Why Use Chrome and ONLY Chrome to render FileMaker script PDFs?**  
   We all must use Chrome to document script changes to Help Give Thanks solutions because formatting is lost when you copy from any other PDF viewer that I tested, AND because each PDF viewer parses PDF text differently.  If we all use the same viewer then we only see changes we actually make to these scripts.  If we use different viewers, then we see many fake changes, that are actually just differences in the way different PDF viewers parse PDF text.  So, please use Chrome.  
   
   If you know of a better PDF parser for FileMaker script PDFs, comment below or here, and we'll all test it, and if it is better than I'll replace all scripts with this new PDF viewers rendition of them, and we will use it going forward.  But, until a better solution is found, please use Chrome.

   *18 minutes, 35 seconds* 

   **Commit file changes to GitHub**

9. Copy Specific Action description.
10. Open GitHub application on your computer and go to solution's repository.
11. Paste Specific Action description into description box and summarize changes. 
12. Commit changes. 
13. Sync changes with GitHub repository on the web.  
14. Confirm changes on www.GitHub.com  

*25 minutes, 42 seconds* 

**Documenting Layout/Screen Changes**  
Take and annotate a screenshot of your layout change, making sure to include 
solution window titles in your screenshots. *Annotate your screenshots using the Mac Preview program or Evernote Skitch, which is a free screenshot annotation tool for both Mac and Windows.* Place your screenshot in the changed solution's layoutChanges folder and commit them to GitHub along with any script changes that are part of a commit.   

If conditional formatting was added or changed, log the addition or change in the conditionalFormattingChangeLog.c file located in all solutions' layoutChanges folders.  Instructions for how to log changes are at the top of each conditionalFormattingChangeLog.c file.  

*29 minutes, 50 seconds* 
####C. Commit updated FileMaker files to GitHub
Committing a solution's new FileMaker version with all recent changes allows for easy copy/paste of scripts, layout objects, etc. into previous versions for testing and approval.

**Library**

1. Log into Library file as admin user: username = admin, password = 4/1/2012beta
2. Run creatEmptyLibrary script.
  1. Name new file with latest Library commit number at https://github.com/HelpGiveThanks/Library.
  2. Save file into your local GitHub Library repository folder.
  3. Close the open Library file.
  4. Go to new Library file and open it. Ignore inability to find reference file: click cancel button.
  5. Click proceed button to proceed with emptying of copied Library file (do make sure that you are indeed emptying the new copy of your Library file and not your original!).
  6. Close copy.  FYI: When opened again, this newly created empty Library asks if you want to start a new Library or import a Library from older version of the Library solution. 
3. Compress/Zip file.
4. Delete uncompressed file.
5. Go to GitHub App and type reason for new FileMaker file including copied commit number.
6. Commit new file.
7. Sync commit.
8. Go to GitHub on the web to confirm commit. 
  
*34 minutes, 37 seconds* 

**ActionLog**

1. Copy most recent commit number from https://github.com/HelpGiveThanks/ActionLog
2. Copy your improved ActionLog file.
3. Paste it into your local GitHub ActionLog repository ActionLog sub folder.  The ActionLog consists of three related databases each with their own folder in the main ActionLog repository folder: ActionLog, MyData, Reference. 
4. Replace file name with copied, most-recent commit number (only need first part of number for identification purposes). 
5. Compress/Zip file.
6. Delete uncompressed file.
7. Go to GitHub App and type reason for new FileMaker file including the full, copied, commit number.
8. Commit new file.
9. Sync commit.
10. Go to GitHub on the web to confirm commit. 
  
**Other Solutions: Help, HeartWhisperer, Budget Planner, IQ Raiser**  
At this time, I have not created an import script and process for these solutions, which like the Library are one database containing both layouts, scripts, and user data.  So, if you improve them, please do what you can to reduce their file size such as removing user data if it will help, compress/zip them, and delete the unzipped file before making your commit.  
  

