# Notes for 1st lesson

## Programming skill
| Time          | Language      | pros           | 
| ------------- |:-------------:| --------------:|
| Week1-5       | Linus (bash)  | string process |
| Week6-16      | R             | data matrix    |

## Bioinformation&Genomics
### 1. Gene:
   * A segment fo information, can be DNA or RNA or other kinds of things
### 2. Human genome:
   * about 3Gb but only 2w genes
   * most are "junk DNA"
   * However, it appears to be that 75% of human genome can be transcripted
   * But only 2-3% can be translated into proteins
### 3. Genes:
   * coding and noncoding genes
### 4. RNAs:
   * the timeline for RNA discovery
   * mRNA -> tRNA/rRNA -> mi-RNA -> LincRNAs
### 5. The main feature for bioinformatics discovery
   * from DATA to CONCLUSION
   * especially big&high dimensional data

## Docker-Setup
### 1. get an image:
   * docker load -i route (本地)
   * docker pull image （下载）
### 2. run a container:
   * mkdir ~/Desktop/bioinfo_tsinghua_share
   * docker run --name=bioinfo_tsinghua -dt  -h bioinfo_docker --restart unless-stopped -v ~/Desktop/bioinfo_tsinghua_share:/home/test/share xfliu1995/bioinfo_tsinghua:2
   * -dt --restart unless-stopped: 设置该_container_能一直在后台保持运行状态
   * -v ~/Desktop/bioinfo_tsinghua_share:/home/test/share: 将宿主机的目录~/Desktop/bioinfo_tsinghua_share作为数据卷挂载到_container的/home/test/share目录下。docker通过数据卷(volume)实现宿主机和container之间的文件同步。我们在container_中修改/home/test/share目录下的内容，就相当于修改宿主机~/Desktop/bioinfo_tsinghua_share目录下的内容。
### 3. use and exit a container:
   * 运行_container_: 在Terminal中输入 docker exec -it bioinfo_tsinghua bash 。(-it,交互式)
   * 退出_container_：exit

## Linux
### 1. Basic command
* linux中有三剑客之称：
* grep ： 过滤文本
* sed  :  修改文本
* awk  :  处理文本

     

# Plan for this semester
| Time          | Language      | Material                         | 
| ------------- |:-------------:| --------------------------------:|
| Week1-5       | Linus (bash)  | take classes, tutorial, practice |
| Week6-16      | R             | take classes, tutorial, practice |
| Week11-16     | Python        | take classes, tutorial, practice |

