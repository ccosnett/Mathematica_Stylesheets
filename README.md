# Mathematica_Stylesheets
mathematica stylesheet which enables print quality math typesetting.

![Screenshot from 2021-05-03 14-23-41](https://user-images.githubusercontent.com/15061801/116881469-33516980-ac1b-11eb-90da-b2a523b8fac3.png)



To install put stylesheet in  `FileNameJoin[{$UserBaseDirectory, "SystemFiles", "FrontEnd", "StyleSheets"}];`

If directory does not exist then run:

    dir = FileNameJoin[{$UserBaseDirectory, "SystemFiles", "FrontEnd", "StyleSheets"}];
    If[! DirectoryQ[dir], CreateDirectory[dir]];
    

Then execute:

    CurrentValue[$FrontEnd, DefaultStyleDefinitions] = "DefaultModified2.nb";
    
    
To copy directory path to clipboard execute:

    CopyToClipboard[FileNameJoin[{$UserBaseDirectory, "SystemFiles", "FrontEnd", "StyleSheets"}]]
    
    
## font size

Preferences -> Global Font Size = 200%


## inline math 


copy and paste current style in style sheet and then edit into this form:

    Cell[StyleData["InlineCell"],
     TextAlignment->Left,
     LanguageCategory->"Formula",
     ScriptLevel->1,
     StyleMenuListing->None,
     FontFamily->"Times",
     FontSize->12]
