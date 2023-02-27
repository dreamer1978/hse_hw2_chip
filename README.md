# hse_hw2_chip

Скачивем необходимые файлы для работы с выбранными клеточной линией и гистоновой меткой.

```
# ChIP-seq на гистоновой метке
# ENCFF889AII
!wget https://www.encodeproject.org/files/ENCFF889AII/@@download/ENCFF889AII.fastq.gz
# ENCFF500BZD
!wget https://www.encodeproject.org/files/ENCFF500BZD/@@download/ENCFF500BZD.fastq.gz

# ChIP-seq контроль
# ENCFF282SBH for ENCSR503UNI
!wget https://www.encodeproject.org/files/ENCFF282SBH/@@download/ENCFF282SBH.fastq.gz
```

Затем смотрим качество чтений. Оно в целом не очень хорошее.
![Screenshot](ENCFF889AII_fastqc.png)
![Screenshot](ENCFF500BZD_fastqc.png)
![Screenshot](ENCFF282SBH_fastqc.png)
Применяем подрезание чтений.
![Screenshot](ENCFF889AII_trimmed.png)
![Screenshot](ENCFF500BZD_trimmed.png)
![Screenshot](ENCFF282SBH_trimmed.png)
Качество чтений улучшается.