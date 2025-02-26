<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aplikasi Perhitungan Diskon</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-5">
   <div class="row justify-content-center">
    <div class="col-md-6">
     <div class="card">
      <div class="card-header">
  <h3 class="text-center"> Aplikasi Perhitungan Diskon</h3>
   </div>
    <div class="card-body">
     <form method="post">
      <div class="mb-3">
   <label for="harga" class="form-label">Harga Barang (Rp)</label>
   <input type="number" class="form-control" id="harga" name="harga" placeholder="Masukkan harga barang" required>
     </div>
      <div class="mb-3">
   <label for="diskon" class="form-label">Diskon (%)</label>
   <input type="number" class="form-control" id="diskon" name="diskon" min="0" max="100" maxlength="3" placeholder="Masukkan diskon (0 - 100" oninput="if(this.value > 100) this.value = 100; if(this.value.length > 3) this.value = this.value.slice(0,3)" required>
    </div>
   <button type="submit" class="btn btn-primary w-100">Hitung</button>
     </form>
        
 <?php
 if ($_SERVER["REQUEST_METHOD"] == "POST") {
   $harga = $_POST['harga'];
   $diskon = $_POST['diskon'];
                            
   $jumlahDiskon = $harga * ($diskon / 100);
   $hargaAkhir = $harga - $jumlahDiskon;
                            
     echo '<div class="mt-4">';
     echo '<h4>Hasil Perhitungan:</h4>';
     echo '<p>Harga Awal:<b> Rp ' . number_format($harga, 0, ',', '.') . '</b></p>';
     echo '<p>Diskon:<b> ' . $diskon . '%</b>';
     echo '<p>Jumlah Diskon:<b> Rp ' . number_format($jumlahDiskon, 0, ',', '.') . '</b>';
     echo '<p>Harga Akhir:<b> Rp ' . number_format($hargaAkhir, 0, ',', '.') . '</b></p>';
     echo '</div>'; }
 ?>
       </div>
      </div>
     </div>
    </div>
   </div>  
 
  <footer class="text-center p-3 text-muted">
   <small>&copy; TUGAS | Nama Siswa | Kelas</small>
   </footer>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
