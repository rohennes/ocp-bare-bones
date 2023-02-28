# Testing two packages with a single .vale.ini file 

The goal is to test if we can have a single .vale.ini file that includes multiple styles. And that different text editors lint these different styles as expected. 

The .vale.ini file is in the parent directory, and applies one style to the this directory, and an additional style to the child directory. 

welcome/index.adoc should have an AsciiDoc error and a RedHat error:
* AsciiDoc.ValidTableBlocks
* RedHat.TermsSuggestions

index.adoc should only have the RedHat error:
* RedHat.TermsSuggestions

![image](https://user-images.githubusercontent.com/104497497/221920853-bd0ffaca-11f6-4df6-911b-d1fc7cb0ed60.png)
