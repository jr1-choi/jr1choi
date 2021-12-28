# jr1choi

SOP
12/23/2021 ver.1.0
 
1. CKDgen Meta-Analysis Data 접속.
https://ckdgen.imbi.uni-freiburg.de/

2. Urate 관련 화일 다운로드 – 저자, 파일 이름, 크기 등 확인

Author

Schlosser et al. 2021
UACA

Tin et al. 2021
Urate

Tin et al. 2019
Urate, trans-ethnic
Urate, European-American ancestry

Teumer et al. 2019
UACR overall, trans-ethnic
UACR Diabetes mellitus, trans-ethnic
UACR overall, European-American ancestry
UACR overall, African-American ancestry

Li et al. 2017
UACR EA
UACR AA

일본 요산 GWAS
hum0167.v1.meta.v1

대만 요산 GWAS
URIC_ACID. Assoc.linear.gz

 

3. 찾기로 terminal 열어서

jungranchoi@Jungui-iMac ~ % pwd
/Users/jungranchoi
jungranchoi@Jungui-iMac ~ % cd ..desktop
cd: no such file or directory: ..desktop
jungranchoi@Jungui-iMac ~ % cd desktop
jungranchoi@Jungui-iMac desktop % cd CKD
jungranchoi@Jungui-iMac CKD % ls     
Published_UACR_AA.csv
Published_UACR_EA.csv
UACR.csv
formatted_20170020-UACR_DM-All-nstud_18-SumMac_400.tbl.rsid
formatted_20170711-UACR_overall-ALL-nstud_27-sumMac_400.tbl.rsid
formatted_20180202-UACR_overall-AA-nstud_1-SumMac_400.rsid.tbl
formatted_20180517-UACR_overall-EA-nstud_18-SumMac_400.tbl.rsid
urate.csv
urate_chr1_22_LQ_IQ06_mac10_EA_60_prec1_nstud30_summac400_rsid.txt
urate_chr1_22_LQ_IQ06_mac10_all_741_nstud37_summac400_rsid.txt
jungranchoi@Jungui-iMac CKD % head -10 formatted_20170020-UACR_DM-All-nstud_18-SumMac_400.tbl.rsid
Chr Pos_b37 RSID Allele1 Allele2 Freq1 Effect StdErr P-value n_total_sum
1 751756 rs28527770 t c 0.7830 0.0003 0.0166 0.9849 15099
1 752566 rs3094315 a g 0.7985 0.0032 0.0096 0.7363 40304
1 752721 rs3131972 a g 0.2041 -0.0058 0.0097 0.5517 39376
1 752894 rs3131971 t c 0.2136 -0.0201 0.0158 0.2012 14571
1 753405 rs3115860 a c 0.8370 -0.0041 0.0105 0.698 39784
1 753541 rs2073813 a g 0.1528 0.0028 0.0108 0.7958 38016
1 754182 rs3131969 a g 0.1620 0.0025 0.0107 0.818 38288
1 754192 rs3131968 a g 0.1618 0.0014 0.0107 0.8968 38288
1 754334 rs3131967 t c 0.1616 -0.0004 0.0108 0.9731 37844
jungranchoi@Jungui-iMac CKD % tail -10 formatted_20170020-UACR_DM-All-nstud_18-SumMac_400.tbl.rsid
22 51171693 rs756638 a g 0.2823 0.0102 0.0074 0.1688 49544
22 51175626 rs3810648 a g 0.9184 0.0036 0.0127 0.7777 49880
22 51178090 rs2285395 a g 0.0603 -0.0058 0.0139 0.6759 49649
22 51182399 rs56238942 a g 0.9150 0.0188 0.0138 0.1739 38527
22 51186228 rs3865766 t c 0.4571 -0.0060 0.0079 0.4472 36011
22 51186276 rs8135434 t c 0.9208 0.0074 0.0146 0.613 38527
22 51212875 rs2238837 a c 0.6459 -0.0027 0.0086 0.7545 35066
22 51213613 rs34726907 t c 0.1458 -0.0163 0.0111 0.1412 37255
22 51216564 rs9616970 t c 0.8626 0.0182 0.0112 0.1044 37042
22 51219006 rs28729663 a g 0.1576 -0.0204 0.0109 0.06142 35795
jungranchoi@Jungui-iMac CKD % wc -l formatted_20170020-UACR_DM-All-nstud_18-SumMac_400.tbl.rsid
 6824034 formatted_20170020-UACR_DM-All-nstud_18-SumMac_400.tbl.rsid
 

1 pwd : directory 확인  
- jungranchoi@Jungui-iMac ~ % pwd
2) cd desktop - 화일 있는 폴더 위치
- 현재 디렉토리 상향 – cd 화일 위치
- 현재 디렉토리 하향 – cd ..
예. jungranchoi@Jungui-iMac ~ % cd desktop - 데스크탑 위치 확인
예. jungranchoi@Jungui-iMac desktop % cd CKD - 데스크탑 CKD 폴더
5) jungranchoi@Jungui-iMac CKD % ls - 폴더 내 파일 리스트 확인
6) jungranchoi@Jungui-iMac CKD % head -10 화일명 (formatted_20170020-UACR_DM-All-nstud_18-SumMac_400.tbl.rsid)
- 화일 앞 10줄 확인
7) jungranchoi@Jungui-iMac CKD % tail -10 화일명(formatted_20170020-UACR_DM-All-nstud_18-SumMac_400.tbl.rsid)
- 파일 마지막 10줄 확인
8) jungranchoi@Jungui-iMac CKD % wc -l 화일명(formatted_20170020-UACR_DM-All-nstud_18-SumMac_400.tbl.rsid)
- 전체 SNP 수 확인
9)  6824034 formatted_20170020-UACR_DM-All-nstud_18-SumMac_400.tbl.rsid
- SNP 수 6824033
