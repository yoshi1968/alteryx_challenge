# Challenge499

## Project Name: Weekly Challenge #499: Where is Waldo?
- [Source](https://community.alteryx.com/t5/Weekly-Challenges/Challenge-499-Where-is-Waldo/td-p/1427290/page/5)
- [My solution](https://community.alteryx.com/t5/Weekly-Challenges/Challenge-499-Where-is-Waldo/m-p/1431672/highlight/true#M154460)

## Summary
    Read .xlsx files under "Places" directory 
    Find a sheet where "Is Waldo here?" = "Y"

## Workflow

![Workflow](Challenge499-wf.png)

## Main Process
- Step1: Read parent directory
- Step2: Edit full path to read <List of Sheet Names>
- Step3: Get the list of sheet names
- Step4: Read all the sheets
- Step5: Filter "Is Waldo here?"
- Step6: Parse full path to get Folder/Subfolder/File/Sheet

## Last Update
2026-02-16

