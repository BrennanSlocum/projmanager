# projmanager by blue: 1.4.3 @ August 06, 2026
[![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnubash&logoColor=fff)](#)
[![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?logo=github&logoColor=white)](#)

personal project manager
## tools:
- archive projects (-z)
- update projects to /usr/local/bin (-u)
- update project versions (-p)
- generate and remove new projects (-g & -r)
- open config (-c)
- lint (-l) (literally only uses shellcheck)
...and hopefully more soon?

## config options
root: this is the root folder for your projects.
projects: the directory of your project (root/foo, root/bar)
archive: directory to put project archives

```bash
projmanager -z <project-name>
```
...zips projects to archive with date

```bash
projmanager -u <project-name>
```
...updates local (root/project-name) to global (/usr/local/bin)

```bash
projmanager -p -u <project-name>
```
...updates and prompts for new version (writes to the FIRST LINE in a readme file)

```bash
projmanager -g <project-name>
```
...adds a new project (generates readme, sample code, etc...)
projmanager -r does the opposite

```bash
projmanager -c 
```
...opens config

## todo
- [ ] -i import option for -z
