# leb3web
<p>Nama  : Muhamad valentino ramzi</p>
<p>Nim   : 312410454</p>
<p>Kelas : TI.24.A5</p>

## 🧩 Praktikum 3: Membuat List, Table, dan Form

### **1️⃣ Membuat Ordered List**

```html
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
        <li>Pemrograman Web</li>
        <li>Sistem Informasi</li>
        <li>Basis Data 2</li>
    </ol>
</section>
```

**Penjelasan perubahan:**

<img width="682" height="276" alt="t_1" src="https://github.com/user-attachments/assets/83ca0737-df44-4b12-adc4-7437ed9045dc" />



* Tag `<section>` digunakan untuk mengelompokkan bagian list.
* Tag `<ol>` (ordered list) berfungsi menampilkan daftar berurutan (nomor 1, 2, 3…).
* Tag `<li>` berisi setiap item list.
* Tambahan `id="order-list"` berfungsi untuk penandaan atau pemanggilan CSS.

---

### **2️⃣ Membuat Unordered List**

```html
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```

**Penjelasan perubahan:**

<img width="705" height="494" alt="t_2" src="https://github.com/user-attachments/assets/6dda2d95-3ea7-4bdf-93e0-e9715d92a2cf" />



* Menggunakan `<ul>` (unordered list) untuk menampilkan daftar tidak berurutan.
* Atribut `type="square"` mengubah simbol default (lingkaran) menjadi kotak.
* Karakter `&amp;` digunakan agar tanda “&” bisa tampil dengan benar di browser.

---

### **3️⃣ Membuat Description List**

```html
<section id="description-list">
    <h2>Description List</h2>
    <dl>
        <dt>Fakultas Teknik</dt>
        <dd>Teknik Industri</dd>
        <dd>Teknik Informatika</dd>
        <dd>Teknik Lingkungan</dd>
        <dt>Fakultas Ekonomi dan Bisnis</dt>
        <dd>Akuntansi</dd>
        <dd>Manajemen</dd>
        <dd>Bisnis Digital</dd>
    </dl>
</section>
```

**Penjelasan perubahan:**

<img width="683" height="606" alt="t_3" src="https://github.com/user-attachments/assets/481b2e8f-f4dc-4472-a69c-3d2cf5ae5cdf" />


* `<dl>` = description list, berisi pasangan istilah dan penjelasannya.
* `<dt>` = judul istilah (misalnya nama fakultas).
* `<dd>` = deskripsi atau rincian dari istilah (misalnya jurusan).
* Ini menunjukkan hubungan hierarki antara data utama dan subdata.

---

### **4️⃣ Membuat Tabel**

```html
<table border="1" cellpadding="4" cellspacing="0">
    <thead>
        <tr>
            <th>No.</th>
            <th>Fakultas</th>
            <th>Program Studi</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td>Teknik</td>
            <td>Teknik Informatika</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Teknik</td>
            <td>Teknik Industri</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>Teknik</td>
            <td>Teknik Lingkungan</td>
        </tr>
    </tbody>
</table>
```

**Penjelasan perubahan:**

<img width="763" height="318" alt="t_4" src="https://github.com/user-attachments/assets/23d25b1d-9943-4ac0-87a3-1015db5838bb" />



* `<table>` mendefinisikan tabel utama.
* Atribut `border`, `cellpadding`, dan `cellspacing` digunakan untuk memperindah tampilan (garis & jarak antar sel).
* `<thead>` dan `<tbody>` memisahkan bagian kepala dan isi tabel.
* `<th>` digunakan untuk judul kolom.
* `<tr>` untuk baris, `<td>` untuk kolom isi.

---

### **5️⃣ Menggabungkan Sel Data**

```html
<td rowspan="3">Teknik</td>
```

**Penjelasan perubahan:**

<img width="661" height="246" alt="t_5" src="https://github.com/user-attachments/assets/9cdcde8f-000d-48d1-8dca-15bab14a865f" />


* Atribut `rowspan="3"` digunakan untuk menggabungkan 3 baris pada kolom fakultas “Teknik”.
* Tujuannya agar data tidak ditulis berulang kali dan tampilan lebih rapi.

---

### **6️⃣ Membuat Form**

```html
<form action="proses.php" method="post">
    <fieldset>
        <legend>Data Pelanggan</legend>
        <p>
            <label for="nama">Nama</label>
            <input type="text" id="nama" name="nama">
        </p>
        <p>
            <label for="alamat">Alamat</label>
            <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
        </p>
        <p>
            <label>Jenis Kelamin</label>
            <input id="jk_l" type="radio" name="kelamin" value="L" /><label for="jk_l">Laki-laki</label>
            <input id="jk_p" type="radio" name="kelamin" value="P" /><label for="jk_p">Perempuan</label>
        </p>
        <p><input type="submit" value="Login"></p>
    </fieldset>
</form>
```

**Penjelasan perubahan:**

<img width="1022" height="365" alt="t_6" src="https://github.com/user-attachments/assets/7bd1c66b-80ed-497a-9d3d-b88d78960919" />


* `<form>` digunakan untuk mengumpulkan data dari pengguna.
* `action="proses.php"` menentukan file yang akan menerima data.
* `method="post"` mengirim data secara tersembunyi (tidak terlihat di URL).
* `<fieldset>` membuat batas area form, `<legend>` memberi judul.
* `<label>` memberi keterangan untuk input, `<input>` dan `<textarea>` untuk pengisian data.
* Input radio (`type="radio"`) digunakan agar pengguna memilih satu opsi saja.
* Tombol submit (`type="submit"`) digunakan untuk mengirimkan data form.

---

### **7️⃣ Menambahkan CSS ke Form**

```html
<style>
    form p > label {
        display: inline-block;
        width: 100px;
    }
    form input[type="text"], form textarea {
        border: 1px solid #197a43;
    }
    form input[type="submit"] {
        border: 1px solid #197a43;
        background-color: #197a43;
        color: #ffffff;
        font-weight: bold;
        padding: 5px 15px;
    }
</style>
```

**Penjelasan perubahan:**

<img width="585" height="393" alt="t_8" src="https://github.com/user-attachments/assets/e4243acd-a879-42c2-9a3e-c910573e86de" />


* Menambahkan CSS agar tampilan form lebih rapi.
* `display: inline-block; width: 100px;` membuat label sejajar dan rata kiri.
* `border` memberi garis pada input dan tombol.
* `background-color` dan `color` mengatur warna tombol.
* `padding` menambah ruang dalam tombol agar lebih proporsional.

---
# Hasil dropdown menu dan listbox dengan multiple selection.

**Code**

  <!-- Dropdown (Pilih Fakultas) -->
            <p>
                <label for="fakultas">Fakultas</label>
                <select id="fakultas" name="fakultas">
                    <option value="">-- Pilih Fakultas --</option>
                    <option value="teknik">Teknik</option>
                    <option value="ekonomi">Ekonomi dan Bisnis</option>
                    <option value="hukum">Hukum</option>
                    <option value="kedokteran">Kedokteran</option>
                </select>
            </p>

            <!-- Listbox (Pilih Program Studi) -->
            <p>
                <label for="prodi">Program Studi</label>
                <select id="prodi" name="prodi[]" multiple size="4">
                    <option value="ti">Teknik Informatika</option>
                    <option value="ti">Teknik Industri</option>
                    <option value="tl">Teknik Lingkungan</option>
                    <option value="ak">Akuntansi</option>
                    <option value="manajemen">Manajemen</option>
                </select>
            </p>

---
**Hasil**
            
<img width="768" height="529" alt="t_9" src="https://github.com/user-attachments/assets/34e00656-aecc-46d4-a91b-2a9d041ad777" />



