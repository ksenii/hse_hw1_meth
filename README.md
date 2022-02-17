# hse_hw1_meth


○	SRR5836473 - 8 Cell

○	SRR3824222 - Epiblast

○	SRR5836475 - ICM


Сылка на Google Collab: https://colab.research.google.com/drive/1M4if3EnAGD5LTrbSNl7U73l1czCW0k-Y?hl=ru#scrollTo=b9Pfcq4ZYb_T

Задание #1
=====================


Задание #2
=====================

### Пункт а
Работа с bam-files с выравниваниями BS-seq ридов на 11-ю хромосому мыши

Ниже представлена сводная таблица с числом ридов, закартированных на участки
1) 11347700-11367700
2) 40185800-40195800

![alt text](image/a.png)


### Пункт b
Результаты дедупликации файлов выравниваний (в %).

![alt text](image/b.png)

Скрипт для выполнения дедупликации для всех образцов одновременно:
! ls SRR5836475_1_bismark_bt2_pe.bam SRR3824222_1_bismark_bt2_pe.bam SRR5836473_1_bismark_bt2_pe.bam | xargs -P 3 -tI{} deduplicate_bismark  --bam  --paired  -o s_{} {}
#### Результат:
.......

Total number of alignments analysed in SRR5836473_1_bismark_bt2_pe.bam:	2850231
Total number duplicated alignments removed:	521904 (18.31%)
Duplicated alignments were found at:	230432 different position(s)
Total count of deduplicated leftover sequences: 2328327 (81.69% of total)


Total number of alignments analysed in SRR5836475_1_bismark_bt2_pe.bam:	4159998
Total number duplicated alignments removed:	377882 (9.08%)
Duplicated alignments were found at:	229833 different position(s)
Total count of deduplicated leftover sequences: 3782116 (90.92% of total)


Total number of alignments analysed in SRR3824222_1_bismark_bt2_pe.bam:	7039016
Total number duplicated alignments removed:	205258 (2.92%)
Duplicated alignments were found at:	164796 different position(s)
Total count of deduplicated leftover sequences: 6833758 (97.08% of total)

.......

### Пункт c
Сделано в Google Collab 

### Пункт d



### Пункт e


### Пункт f
