
Project3-IndonesiaAI
# Segmentation-for-Self-Driving-Car-using-U-Net

**Background & Problem Statement**
- Segmentasi Gambar adalah proses mempartisi gambar digital menjadi beberapa segmen gambar yang juga dikenal sebagai wilayah gambar atau objek gambar (kumpulan piksel). Tujuan dari segmentasi adalah untuk menyederhanakan dan/atau mengubah representasi gambar menjadi sesuatu yang lebih representatif dan lebih mudah untuk dianalisis. Segmentasi gambar sering digunakan untuk menemukan objek dan batas-batasnya.
- Masalah umum di banyak kota besar di dunia adalah kemacetan lalu lintas dan tingginya jumlah kecelakaan. Salah satu faktor yang berperan besar dalam terjadinya insiden ini adalah kelalaian pengemudi.
- Menurut WHO, sistem lalu lintas adalah salah satu sistem yang paling kompleks dan berbahaya yang kita hadapi hampir setiap hari
- Dengan konsep Mobil Mandiri (Self-Driving Car), diharapkan dapat mengurangi jumlah kecelakaan dan kemacetan akibat kelalaian pengemudi.
  
**Objective**

  - Segmentasi self driving car menggunakan teknik deep learning yaitu U-Net untuk mengurangi jumlah kecelakaan dan kemacetan akibat kelalaian pengemudi
    
  **Dataset**
  
    - Dataset yang digunakan merupakan data Cityscapes Dataset yang memuat gambar-gambar citra kamera https://www.cityscapes-dataset.com/
      Data Training : 367 gambar
      Data Testing : 101 gambar
    - class Data: 0= Background; 1. Sky; 2. Building; 3. Pole; 4. Road; 5. Pavement;  6. tree; 7. SignSymbol; 8. Fence; 9. Car; 10. Pedestrian; 11. Bicyclist
      
  **Preprocessing**
  
   - Normalize data train dan data testing
     
  **Arsitektur U-Net**
  
![image](https://github.com/fenchi-riti/Segmentation-for-Self-Driving-Car-using-U-Net/assets/72839436/e2502c61-450f-4c9a-8b04-a5c4c0486c9f)
- U-Net adalah jaringan saraf konvolusional yang dikembangkan untuk segmentasi gambar biomedis di Departemen Ilmu Komputer Universitas Freiburg. Jaringan ini didasarkan pada jaringan konvolusional penuh dan arsitekturnya dimodifikasi dan diperluas untuk bekerja dengan lebih sedikit gambar pelatihan dan menghasilkan segmentasi yang lebih tepat.
  
  **Training Model**
  
  Optimizer : Adam; Learning rate: 0.001
  Batch Size : 4
  Loss function : categorical crossentropy
  Epoch : 100
  Training accuracy : 0.92
  Validation accuracy : 0.85
  Training Loss : 0.2486
  Validation Loss : 0.6
Accuracy   ![image](https://github.com/fenchi-riti/Segmentation-for-Self-Driving-Car-using-U-Net/assets/72839436/0e5f4fb7-7c10-4351-828b-39f11bf30c51) ![image]

Loss (https://github.com/fenchi-riti/Segmentation-for-Self-Driving-Car-using-U-Net/assets/72839436/84ddcbf6-9bda-43ba-9909-10ce9393f3b3)

**Testing Model**
  Test Loss : 0.8
  Test accuracy: 0.78
  
  Grafik IoU setiap Class ![image](https://github.com/fenchi-riti/Segmentation-for-Self-Driving-Car-using-U-Net/assets/72839436/7fb97c95-9c4e-4d7d-8f62-720db1e1e2f3)
  
**Experiment**
Accuracy  ![image](https://github.com/fenchi-riti/Segmentation-for-Self-Driving-Car-using-U-Net/assets/72839436/33c4ecf1-9837-49a0-8f53-49287776b928)
Loss ![image](https://github.com/fenchi-riti/Segmentation-for-Self-Driving-Car-using-U-Net/assets/72839436/c367d639-c2b0-4851-b725-09328ca992bd)
IoU ![image](https://github.com/fenchi-riti/Segmentation-for-Self-Driving-Car-using-U-Net/assets/72839436/4b01dbe5-bd1b-4c7c-aa9f-cf9800cc05ab)





  








      
