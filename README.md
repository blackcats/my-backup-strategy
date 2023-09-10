# My Backup Strategy

<!-- put some badge here -->
![Static Badge](https://img.shields.io/badge/ansible-vX.Y.Z-red)
<!-- ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/blackcats/my-backup-strategy/toto.yml?logo=GitHub) -->

This is the main part of my backup strategy [project](https://github.com/users/blackcats/projects/5/views/3).

<!-- Optional: put a table of content -->

## Project status
This project have not yet started. Development should begin in the next few
weeks, I hope. I still have a couple of things to think about before I get 
started.

## About the project
<!-- This section  may be Optional and fusioned with the description. -->
This repository contain the scripts for my _new backup strategy_, with some 
explainations.

A backup strategy is something everyboby must have and these must reflect his 
needs. 

I have personally been using the 3-2-1 backup strategy for many years.
```
3 copies of my datas
2 copies on different storage media
1 offsite copy
```

For many years, I have been using a NAS with RAID and external hard drives as
a backup system for years. I had scripts on my systems that were run every 
night to back up my data to the NAS, and on the NAS a program to back up data 
to external hard drives. These disks were moved out of my home manually every 
week to be replaced by those from the previous week. And it worked well.

But one day the problems started. I became seriouly ill, and could no longer
outsite the hard drives. During this period and after, one of the hard drives 
where I backed up my datas failed. And some time later, a hard drives of my 
NAS failed too during a reconstruction. Arg... It meant:
- 1. no more backups
- 2. a potential loss of datas (thankfully not)

Of these problems, I learned:
- 1. offsite copy must be automatic
- 2. RAID is not a backup...
- 3. Keep a small number of datas version 

So I decided to review my backup strategy:
- 1. Offsite copy will be automated on a AWS S3 bucket
- 2. My NAS will continue to be part of my backup system
- 3. My backup system will be fully automated from a single machine.
And of course, I am going to use the 3-2-1 strategy for my backups.

Ok, that's well and dandy but how I will set up this darn project? 

First I created an AWS S3 bucket to archive my datas. You can see how I set it 
up [here](https://github.com/blackcats/my_freezed_storage). After that...
I'm stil thinking about how I'm going to proceed...

<!-- ## Get Started -->
<!-- if used, this section contain the "Installation" and "Usage" section -->

<!-- ## Installation -->
<!-- Requirement and How to install -->

<!-- ## Usage -->
<!-- How to use the project. Put some example (command and exepted output) -->

<!-- ## Support  -->
<!-- Tell people where they can go to for help. It can be any combination -->
<!-- of an issue tracker, a chat room, an email address, etc... -->

<!-- ## Roadmap (or Todo) -->
<!-- Ideas for futur evolution or missing features -->
<!-- - [ ] Add branch protection rules when the repository will be public -->

<!--## Contributing -->
<!-- How to contribute to the project, Issue, pullrequest... -->

## Acknowledgment
I would like to thank [geerlingguy](https://github.com/geerlingguy/) for the 
presentation of [his backup strategy](https://github.com/geerlingguy/my-backup-plan). 
What he says and explains has enabled me to review my own backup strategy, 
and at the same time, to do what I had been putting off for months: _create 
terraform and ansible projects for my needs_, and not just for my work.

## Author
This project was created in 2023 by [Olivier LE GALL](lgo@black-cats.org).

## Licence
This project is under the GNU GPLv3 license.
