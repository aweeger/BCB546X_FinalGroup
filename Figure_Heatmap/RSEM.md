## Environment preparation
```
$ cd /ptmp/aweeger/BCB546X_FinalGroup/
```
```
$ module load rsem/1.3.0-py2-r3.5-6w56sc6
```
```
$ module load  python/3.8.0-k7w5uj4
```
```
$ module load  bowtie2/2.3.4.1-py2-jl5zqym
```
```
$ bowtie2-build HG973349-HG973421.fasta HG973349-HG973421 # builds alignment index using bowtie2
```
```
$ rsem-prepare-reference HG973349-HG973421.fasta HG973349-HG973421 # prepares RSEM reference 
$ mkdir individual
```

## SLURM jobs to run
```
$ sbatch rsem_individual_2430.job # SLURM part 1
```
```
$ sbatch rsem_individual_2431_1.job # SLURM part 2
```
```
$ sbatch rsem_individual_2431_2.job # SLURM part 3
```