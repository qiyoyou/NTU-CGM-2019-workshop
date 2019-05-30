# NTU-CGM-2019-workshop
## Genome-wide association analysis with application in R & PLINK

### R markdown document links:
1. [Basic R command](https://drive.google.com/file/d/1QeyPQ8XLzIM8e306mZYcj9QuzTVEIgZI/view?usp=sharing)
1. [Basic R command](http://drive-html-viewer.pansy.at/?state=%7B%22ids%22:%5B%221QeyPQ8XLzIM8e306mZYcj9QuzTVEIgZI%22%5D,%22action%22:%22open%22,%22userId%22:%22{userId}%22%7D)


<H2>

### Active the environment 
```
source /opt/miniconda3/bin/activate /opt/miniconda3/envs/qy/
```


<H2>

### Data management (with PLINK)
Perform quality control for "rawdata" and PCA for population stratification issue.   
```
plink --bfile /home/train2019/qy/rawdata --geno 0.1 --maf 0.01 --mind 0.05 --hwe 0.000001 --make-bed --pca --out /home/train2019/stu60/qy/qcdata
```
```





