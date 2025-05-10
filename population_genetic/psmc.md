# psmc
是使用单个个体的bam文件和参考序列文件估算历史有效群体大小的软件，需要准备好bam文件和参考序列文件并安装psmc [https://github.com/lh3/psmc](https://github.com/lh3/psmc)

## 编译
```{sh}
cd ./psmc/utils
```
```{sh}
make
```
结束之后可以进psmc的目录检查是否有帮助文档
```{sh}
./psmc -h
```

## bam文件转为fastq格式的一致性序列
```{sh}
bcftools
```
## 将fastq格式转psmcfa格式
```{sh}
fq2psmcfa -q20 diploid.fq.gz > diploid.psmcfa
```
