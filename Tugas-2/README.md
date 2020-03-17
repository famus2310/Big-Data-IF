# Tugas 2

Fadhil Musaad

05111740000116

## DB

### DB Connect

1. Masukkan SQLite connector, DB table selector dan DB Reader.
2. Configure newCensus.sqlite pada connector dan select all pada selector dan klik execute pada end node.
![Workflow](image/workflow_1_1.png)
3. Klik kanan pada DB Reader dan pilih KNIME Data table.
![Data Table](image/ss_1_1_1.png)

### In DB Processing

1. Masukkan node-node nya hingga menjadi workflow seperti ini dan klik execute pada end node.
![Workflow](image/workflow_1_2.png)
2. Klik kanan pada DB reader dan pilih KNIME data table
3. Pada data 3, tidak ada hasil yang diquery
![Data Table 1](image/ss_1_2_1.png)
![Data Table 2](image/ss_1_2_2.png)
![Data Table 3](image/ss_1_2_3.png)
![Data Table 4](image/ss_1_2_4.png)

### Modelling

1. Masukkan node-node nya hingga menjadi workflow seperti ini dan klik execute pada end node.
![Workflow](image/workflow_1_3.png)
2. Untuk melihat hasil decision tree nya, klik kanan pada predictor dan view decision tree.
![Decision Tree](image/ss_1_3_1.png)

### Writing to DB

1. Masukkan node-node nya hingga menjadi workflow seperti ini dan klik execute pada end node.
![Workflow](image/workflow_1_4.png)
2. Cek pada DBeaver file sqlite nya
![DBeaver](image/ss_1_4_1.png)

## Hadoop

### Setup Hive Table

1. Cukup jalankan workflownya dan klik execute pada end node.
![Workflow](image/workflow_2_1.png)
2. Buka DBeaver dan lakukan navigasi ke table yang diinginkan.
!