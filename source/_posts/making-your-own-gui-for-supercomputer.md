---
banner_img: http://y1.ifengimg.com/a/2015_29/c083b0baec24d92_size285_w772_h472.jpg
index_img: http://y1.ifengimg.com/a/2015_29/c083b0baec24d92_size285_w772_h472.jpg
title: Making Your Own GUI for Supercomputer
date: 2022-05-17 15:59:58
updated: 2022-05-17 15:59:58
categories:
  - Technology
keywords:
  - Python
comments: true
---
## Motivation

The supercomputer which the writer use is TH-2. The computer uses Slurm workload manager. Users need to write shell scripts first and change the input file into specific forms. 

```shell
$ sinfo                #check the status of the point
$ yhbatch name .sh               #submit the jobs
$ yhq/ squeue                    #check the status of jobs in the point
$ squeue -u YOURNAME                 #check only your jobs 
$ yhcontrol show jobs XXXX        #check job imformation
$ yhcancel XXXXX                  #kill the job
```

## Preparation

### language

python(Tkinler, paraminko)

The writer decided to use Tkinler to create the GUI window, and use paraminko to send SSH command.