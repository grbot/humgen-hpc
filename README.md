The purpose of these scripts are to show how to use variant calling tools on the UCT hex cluster. It should not be considered as best practice for Human variant calling.

1. Currently Git pulls/updates are not working on Hex. Please copy this repository to your home directory

```
cd 
cp -r /researchdata/fhgfs/cbio/cbio/courses/IBS5004Z/humgen-hpc .
```

2. Modify the *config.txt*. Change the output_dir path to point to location of where your processing would be done.

3. For *fastqc.raw.qsub*. Change the PBS -d path with yours, change the location of the config file with yours, change the email address with yours. Then run *qsub fastqc.raw.qsub*

4. For *bwa_mem.raw.qsub*. Change the PBS -d path with yours, change the location of the config file with yours, change the email address with yours. Then run *qsub bwa_mem.raw.qsub*

5. For *mark_duplicates.bwa_mem.raw.qsub*. Change the PBS -d path with yours, change the location of the config file with yours, change the email address with yours. Then run *qsub mark_duplicates.bwa_mem.raw.qsub*

6. For *gatk_hc.mark_duplicates.bwa_mem.raw.qsub*. Change the PBS -d path with yours, change the location of the config file with yours, change the email address with yours. Then run *qsub gatk_hc.mark_duplicates.bwa_mem.raw.qsub*

7. For *gatk_select_snps.hc.mark_duplicates.bwa_mem.raw.qsub*. Change the PBS -d path with yours, change the location of the config file with yours, change the email address with yours. Then run *qsub gatk_select_snps.hc.mark_duplicates.bwa_mem.raw.qsub*

8. For *gatk_filter.select_snps.hc.mark_duplicates.bwa_mem.raw.qsub*. Change the PBS -d path with yours, change the location of the config file with yours, change the email address with yours. Then run *qsub gatk_filter.select_snps.hc.mark_duplicates.bwa_mem.raw.qsub*
