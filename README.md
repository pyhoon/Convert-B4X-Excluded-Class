# Convert Class.bas to Class.b4x_excluded

This script converts file with *.bas extension to *.b4x_excluded to be included into B4X library or B4X Template as class template.

The following lines are not visible inside B4J Code Editor but are visible if you open the *.bas file using a text editor.
```B4X
B4J=true
Group=Handlers
ModulesStructureVersion=1
Type=Class
Version=10.5
@EndOfDesignText@
```

In order to use as a class template, line of code as seen above need to be removed. This script will remove the lines for us so we don't need to edit the files one by one.
## How to use​
1. Download the attached create_excluded.bat file.
2. Put the file at the same path as .b4j project file.
3. The command to run it:
    ```
    create_excluded.bat class1.bas class2.bas
    ```
4. We can use Macro to call this batch file.
### Example
   ```
   #Macro: Title, Create Template, ide://run?File=%PROJECT%\create_excluded.bat&Args=..\Helper.bas
   ```
