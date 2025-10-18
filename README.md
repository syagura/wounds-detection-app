## Setting Up Environment
Setting up local environment for training yolo

### Membuat venv (Opsional tapi Disarankan)
Membuat virtual environment untuk training dan deteksi menggunakan yolo
1. **Membuat venv Menggunakan Python**
   Kita menggunakan python 3.10 untuk project ini, untunk membuat venv menggunakan python gunakan command dibawah
   ```
   python -3.10 -m venv myvenv
   ```
   Setelah membuat venv, aktifkan venv menggunakan command dibawah
   ```
   myenv\Scripts\activate
   ```
2. **Using Conda/Miniconda**
   Jika menggunakan Conda/Miniconda, gunakan command dibawah untuk membuat venv
   ```
   conda create --prefix ./myvenv python=3.10
   ```
   Setelah proses selesai, aktifkan venv menggunakan command berikut
   ```
   conda activate ./venv
   ```

### Cek Nvidia-GPU
Jika laptop menggunakan nvidia cek CUDA version untuk menginstal pytorch sebagai library yang akan digunakan untuk membuat dan load model yolo
Gunakan command berikut untuk cek versi CUDA, buka cmd kemudian masukan command
```
nvidia-smi
```
Setelah itu pada bagian atas akan terlihat versi cuda yang digunakan.

### Install Pytorch
Silahkan buka https://pytorch.org/ kemudian pada instalasi pilih versi cuda sesuai dengan sistem yang dimiliki.
Misalnya seperti ini
```
pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cu126
```
Ubah command tersebut menjadi
```
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu126
```
Tunggu prosesnya hingga selesai
**Note: Proses ini memakan waktu tergantung koneksi internet yang digunakan**

### Install Ultralytics
Untuk mengintsall ultralytics gunakan command dibawah
```
pip install ultralytics
```
tunggu hingga proses selesai

**Environment sudah iap dan bisa lakukan training**
