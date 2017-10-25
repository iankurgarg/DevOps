# CSC5198 - Devops-milestone2
Devops 2 Milestone Testing
### Team Members:
    Debosmita Das(ddas5)
    Abhishek Bandarupalle(abandar)
    Ankur Garg(agarg12)
    Abhimanyu Jataria(ajatari)
    Atit Shetty(akshetty)

## Itrust fork

https://github.ncsu.edu/akshetty/iTrust-v23

branch : fuzzer


## Fuzzer progress

fuzzer.js has main method that takes a directory path and randomly selects a sample list, and modifies them.

runFuzzerJob.js will clone the itrust module, call fuzzer.js and commit the changes.

### Things to add

1) add mvn compile step to verify if the changes are proper.
2) If the changes are proper, commit them else revert the changes.
3) After commiting changes, trigger a jenkins build and moonitor it.


## Analysis 
The report generated by static analyzer (checkbox.io) is present ![here](./analysis/analysis.txt) in txt format and [here](./analysis/analysis_report.xml) in xml format


## Contributions

Ankur Garg (agarg12):
- Analysis Script for checkbox.io for static analysis
- Integration of Analysis script with jenkins build job
- Integration of Useless Test Detector as a post build job of Itrust build job
- Ansible script for fuzzer to run fuzzer on jenkins server
- Ansible Scripts for creating Build jobs of Useless test detector and analysis script
- Creation of specific Ansible Roles for each task.
