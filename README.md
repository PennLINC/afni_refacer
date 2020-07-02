# afni_refacer
 
afni_refacer for refacing T1w (and/or T2w) image 

1. Docker image \
 The docker/singularity image can be pulled from   
`afni_refacer <https://hub.docker.com/repository/docker/pennlinc/afni_refacer>`_ \
`Satterthwaite lab at the University of Pennysilvania
<https://www.satterthwaitelab.com/>`_
Other option is to build from the  dockerfile directly::
```
   docker build -t afni_refacer:latest  - < Dockerfile
  ```

2. Refacing \
T1w or T2w can be refaced with the command below::   
```
   docker run pennlinc/afni_refacer  \
        -input anat_T1w.nii.gz    \
        -mode_reface \
        -prefix anat_T1w_reface.nii.gz
```
