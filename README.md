# Dockerfile for Bridger

A docker container for de novo transcriptome assembly software Bridger.

REF: [Bridger: a new framework for de novo transcriptome assembly using RNA-seq data](http://genomebiology.biomedcentral.com/articles/10.1186/s13059-015-0596-2)

## Usage

Example:

```
$ ls
left.fastq.gz right.fastq.gz
$ docker run -v `pwd`:/data -w /data inutano/bridger:0.1.2 bridger --seqType fq --left /data/left.fastq.gz --right /data/right.fastq.gz --CPU 4
```
