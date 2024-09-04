<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MANCORE NUMFORE</title>
  <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>

  <style>
    /* Gaya umum untuk memastikan ukuran teks responsif */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      padding: 20px;
      background-color: #f0f0f0;
    }

    h1 {
      font-size: 4vw; /* Sesuaikan ukuran berdasarkan lebar viewport */
      text-align: center;
      margin-bottom: 20px;
    }

    label {
      font-size: 1.2em; /* Gunakan em agar ukuran font proporsional */
      margin-right: 10px;
    }

    input {
      padding: 10px;
      font-size: 1em;
      width: 100%;
      max-width: 400px; /* Batas maksimum lebar input */
      box-sizing: border-box;
      margin-bottom: 20px;
    }

    #table_div {
      width: 100%;
      max-width: 98vw; /* Maksimal 90% lebar viewport */
      margin: 0 auto;
      overflow-x: auto; /* Jika terlalu besar, tabel bisa di-scroll */
    }

    /* Gaya tambahan untuk tabel */
    .google-visualization-table-table {
      border-collapse: collapse;
      width: 100%;
    }

    .google-visualization-table-th, 
    .google-visualization-table-td {
      padding: 8px 12px;
      text-align: center; /* Tengah secara horizontal */
      vertical-align: middle; /* Tengah secara vertikal */
      white-space: nowrap; /* Pastikan konten tetap dalam satu baris */
      border: 2px solid #999; /* Tambah ketebalan dan ubah warna garis batas */
    }

    .google-visualization-table-th {
      background-color: #e0e0e0; /* Warna latar belakang header tabel */
    }

    /* Warna latar belakang alternatif untuk baris tabel */
    .google-visualization-table-tr:nth-child(even) {
      background-color: #f9f9f9;
    }

    /* Gaya hover untuk baris */
    .google-visualization-table-tr:hover {
      background-color: #f1f1f1;
    }

    /* Media Queries untuk perangkat dengan layar lebih kecil */
    @media only screen and (max-width: 768px) {
      h1 {
        font-size: 6vw;
      }

      label, input {
        font-size: 1.1em;
      }
    }

    @media only screen and (max-width: 480px) {
      h1 {
        font-size: 8vw;
      }

      label, input {
        font-size: 1em;
      }

      input {
        width: 100%; /* Pada perangkat kecil, input akan memenuhi lebar layar */
      }
    }
  </style>

  <script type="text/javascript">
    // Muat library Google Visualization API
    google.charts.load('current', {'packages':['table']});
    google.charts.setOnLoadCallback(drawTable);

    var data;  // Variabel untuk menyimpan data agar bisa di-filter
    var table; // Variabel untuk menyimpan objek tabel

    function drawTable() {
      // Ganti dengan ID spreadsheet dan gid sheet yang sesuai
      var query = new google.visualization.Query('https://docs.google.com/spreadsheets/d/1kwiMaYyYbv5HCWcymuH13aPdNiZVuqJ92EEV3IEg7_s/gviz/tq?gid=690360252');
      
      // Kirim query untuk mengambil data
      query.send(handleQueryResponse);
    }

    function handleQueryResponse(response) {
      if (response.isError()) {
        alert('Error dalam query: ' + response.getMessage() + ' ' + response.getDetailedMessage());
        return;
      }

      // Simpan data yang diambil
      data = response.getDataTable();

      table = new google.visualization.Table(document.getElementById('table_div'));
      table.draw(data, {showRowNumber: true, width: '100%', height: '100%'});
    }

    // Fungsi untuk melakukan pencarian
    function searchODP() {
      var searchTerm = document.getElementById('searchInput').value.toLowerCase(); // Ambil nilai input pencarian
      var filteredData = new google.visualization.DataTable();

      // Buat struktur tabel baru dengan kolom yang sama
      for (var i = 0; i < data.getNumberOfColumns(); i++) {
        filteredData.addColumn(data.getColumnType(i), data.getColumnLabel(i));
      }

      // Tambahkan baris yang sesuai dengan hasil pencarian
      for (var i = 0; i < data.getNumberOfRows(); i++) {
        var odpNm = data.getValue(i, data.getColumnIndex('ODP_Nm'));

        // Cek apakah ODP_Nm mengandung kata kunci pencarian dan pastikan tidak null
        if (odpNm && odpNm.toLowerCase().includes(searchTerm)) {
          // Ambil setiap nilai kolom di baris dan tambahkan ke tabel yang difilter
          var row = [];
          for (var j = 0; j < data.getNumberOfColumns(); j++) {
            row.push(data.getValue(i, j));
          }
          filteredData.addRow(row); // Tambahkan baris yang cocok ke tabel baru
        }
      }

      // Tampilkan tabel yang sudah difilter
      table.draw(filteredData, {showRowNumber: true, width: '100%', height: '100%'});
    }
  </script>
</head>
<body>
  <h1>MANCORE NUMFORE</h1>

  <!-- Input Pencarian -->
  <label for="searchInput">Cari ODP_Nm:</label>
  <input type="text" id="searchInput" onkeyup="searchODP()" placeholder="Masukkan nama ODP...">

  <!-- Div untuk menampilkan tabel -->
  <div id="table_div"></div>
</body>
</html>
