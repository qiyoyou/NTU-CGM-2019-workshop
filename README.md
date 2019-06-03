# NTU-CGM-2019-workshop
## Genome-wide association analysis with application in R & PLINK

<H2>

### Activate the environment (qy)
```
source /opt/miniconda3/bin/activate /opt/miniconda3/envs/qy/
```


<H2>

### Data management (with PLINK)
Perform quality control for "rawdata" and PCA for population stratification issue. '/home/train2019/qy/' is the path for 'rawdata'; '/home/train2019/${whoami}/qy/' is the path for storing the output which here is named 'qcdata'. You can change the output filename (here is 'qcdata') whatwver you like.
```
plink --bfile /home/train2019/qy/rawdata --geno 0.1 --maf 0.01 --mind 0.05 --hwe 0.000001 --make-bed --pca --out /home/train2019/${whoami}/qy/qcdata
```

<H2>

### R markdown document links:
1. **Basic R command** [[rmd]](https://juuyhcngvzilmlh4agozha-on.drv.tw/CGM%20work/2019_CGM_workshop/WWW/00_Basic_rmd.html) keep updating...

2. **PCA** [[rmd]](https://juuyhcngvzilmlh4agozha-on.drv.tw/CGM%20work/2019_CGM_workshop/WWW/01_PCA_rmd.html)

3. **Analysis** [[rmd]](https://juuyhcngvzilmlh4agozha-on.drv.tw/CGM%20work/2019_CGM_workshop/WWW/02_analysis.html)
