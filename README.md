projmanager by blue: 1.5 @ August 07, 2026
[![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnubash&logoColor=fff)](#)
[![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?logo=github&logoColor=white)](#)

personal project manager
## options:
- -z: archive projects
- -u: update projects to /usr/local/bin
- -U: update project versions
- -g: generate project
- -r: remove project
- -c: open config
- -i: import projects.zip
- -l: lint (literally only uses shellcheck)
- ...and hopefully more soon?

## config options
- root: this is the root folder for your projects.
- projects: the directory of your project (root/project1, root/project2)
- archive: directory to put project archives (see projmanager -z)
- lang: your preferred coding language (generates new projects with this language)

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

```bash
projmanager -i projects.zip
```
...looks for projects.zip and replaces all projects (prompted)

## todo
none :)
