
#pedtools: a robust tool to tidy the complex pedigree with incorrect information and do analysis

## Description

There have been some softwares to deal with mistakes in complex pedigree. But most of them are not robust enough and may be crash in some situations. Further, many softwares are not easy to use to calculate kinship. Pedtools was developed to tidy and display the pedigree. It was robust and can also be used to calculate kinship and summarize the information of progeny.  

## Version

The program was written by C++ and compiled using MinGW 4.9.1 on a 32-bit Windows version. Current version 1.0.1.beta. A GUI version was also available. Please contact P_agro_pmo@genomics.cn if needed.

## Command and option

**Check**   &ensp; &ensp; &ensp; &ensp; pedtools Check [options]

--in           <FILE>    raw pedigree file
--char         <FILE>    checked pedigree file in character format(clean file)
--num          <FILE>    checked pedigree file in numeric format(clean file)
--log          <FILE>    log file,contain information of pedigree error
--drawCircle             draw the error pedigree that the ancestor is progeny at the same time,by default not draw
--branch       <INT>     branch length of dendrogram,default 3
--width        <INT>     name length of individual,default 20


**View** &ensp; &ensp; &ensp; &ensp; &ensp; pedtools View [options]
	
--char         <FILE>    checked pedigree file in character format
--num          <FILE>    checked pedigree file in numeric format
--out          <FILE>    output file
--gender       <CHAR>    gender,default M
--branch       <INT>     branch length of dendrogram,default 5
--width        <INT>     name length of individual,default 20


**Progeny** &ensp; &ensp; &ensp; pedtools Progeny [options]
 
--char         <FILE>    checked pedigree file with character format
--num          <FILE>    checked pedigree file with numeric format
--out          <FILE>    output file

**Kinship** &ensp; &ensp; &ensp; &ensp; pedtools Kinship [options]

--char         <FILE>    checked pedigree file in character format
--num          <FILE>    checked pedigree file in numeric format
--out          <FILE>    output file
--outDir       <FILE>    output directory, work with --outBin
--mode         <CHAR>    animal model or sir model [animal | sir]
--outMatrix              output full matrix,otherwise output binary or lower triangle matrix
--outBin                 output binary kinship
--inbreeding             caluculate inbreeding coefficient


## Contact

If you find bugs please email me.
Author: Zepu Miao  
Email:  miaozepu@genomics.cn  
Institute: Applied agriculture of BGI  


## Licence

Free for research. For commercial use please contact P_agro_pmo@genomics.cn
