# Mathematica_Stylesheets
mathematica stylesheet which enables print quality math typesetting.

![Screenshot from 2021-05-03 14-23-41](https://user-images.githubusercontent.com/15061801/116881469-33516980-ac1b-11eb-90da-b2a523b8fac3.png)



To install put stylesheet in  `FileNameJoin[{$UserBaseDirectory, "SystemFiles", "FrontEnd", "StyleSheets"}];`

If directory does not exist then run:

    dir = FileNameJoin[{$UserBaseDirectory, "SystemFiles", "FrontEnd", "StyleSheets"}];
    If[! DirectoryQ[dir], CreateDirectory[dir]];
    

Then execute:

    CurrentValue[$FrontEnd, DefaultStyleDefinitions] = "DefaultModified.nb";
