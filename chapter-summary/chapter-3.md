# Chapter 3

## Centralized Version Control System

pros:

- help to collaborate with developers
- help to solve administrative questions
- developers know what everyone on the project is doing

cons:

- single point of failure that centralized server represents
- not possible to work without connection to the server
- slow update/commit operations

## Distributed Version Control System

pros:

- each user receive full copy of repository (not only snapshot)
- possible to have more ways of collaboration between different groups of people

## Some of the goals of Git  were as follows

- Speed
- Simple design
- Strong support for non-linear development (thousands of parallel branches)
- Fully distributed
- Able to handle large projects like the Linux kernel efficiently (speed and data size)

## Introduction - Git Foundations

Git uses completely different approach of managing revisions. Git preferes to work with snapshots of work directory [(Snapshots Approach)](https://git-scm.com/book/en/v2/images/snapshots.png) instead of classical approach of saving diffs between revisions [(Diffs Approach)](https://git-scm.com/book/en/v2/images/deltas.png).

Another important feature that inherited by design is to be able to function locally for most of the use cases.

Git uses SHA-1 hash for checksums and changes detection.

When you work with Git files might be in one of the three states [File states in Git](https://git-scm.com/book/en/v2/images/areas.png):

- commited (already saved in local db)
- modified (changed but not saved yet)
- staged (will be included in the next commit)
