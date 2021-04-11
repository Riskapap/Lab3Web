# Praktikum 3 - Pemograman Web
```
Riska Puspa Anggraeni Putri
311910440
TI.19.A2
```
## LANGKAH 1
### Membuat dokumen HTML dengan nama file lab3_list.html. Setelah itu buat struktur dasar HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>HTML Lanjutan</title>
</head>
<body>
 <header>
 <h1>Membuat List</h1>
 </header>
</body>
</html>
```
![1](https://user-images.githubusercontent.com/56241285/114306372-03c0ad00-9b06-11eb-8aaa-95b0ad177b14.png)

## LANGKAH 2
### Membuat Ordered List
```
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
    <li>Pemrograman Web</li>
    <li>Sistem Informasi</li>
    <li>Basis Data 2</li>
    </ol>
  </section>
  ```
  
 ![2](https://user-images.githubusercontent.com/56241285/114306599-7598f680-9b06-11eb-845d-ac4948a6b085.png)

## LANGKAH 3
### Membuat Unordered List
```
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
    <li>Jaringan Komputer</li>
    <li>Struktur Data</li>
    <li>Algoritma &amp; Pemrograman</li>
    </ul>
   </section>
```

![3](https://user-images.githubusercontent.com/56241285/114306719-f3f59880-9b06-11eb-891f-dfcedf0c0937.png)

## LANGKAH 4
### Membuat Description List
```
<section id="unorder-list">
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

![4](https://user-images.githubusercontent.com/56241285/114306883-8d24af00-9b07-11eb-92c7-93fcc1ac5c96.png)

## LANGKAH 5
### Membuat dokumen HTML baru dengan nama file lab3_tabel.html. Setelah itu buat struktur dasar HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>HTML Lanjutan</title>
</head>
<body>
 <header>
 <h1>Membuat Table</h1>
 </header>
</body>
</html>
```
![5](https://user-images.githubusercontent.com/56241285/114307245-f9ec7900-9b08-11eb-851f-ba591008f30b.png)

## LANGKAH 6
### Membuat tabel dan mengatur margin tabel
```
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
![6](https://user-images.githubusercontent.com/56241285/114307489-0b825080-9b0a-11eb-8cf7-81d7f028dd3b.png)

## LANGKAH 7
### Menggabungkan Sel Data
```
<table border="1" cellpadding="6" cellspacing="0">
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
        <td rowspan="3">Teknik</td>
        <td>Teknik Informatika</td>
      </tr>
      <tr>
        <td>2.</td>
        <td>Teknik Industri</td>
      </tr>
      <tr>
        <td>3.</td>
        <td>Teknik Lingkungan</td>
      </tr>
    </tbody>
   </table>
```
![7](https://user-images.githubusercontent.com/56241285/114307662-dcb8aa00-9b0a-11eb-9ba3-9b9288df726c.png)

## LANGKAH 8
### Membuat dokumen HTML baru dengan nama file lab3_form.html dan Buat Tabel
```
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>HTML Lanjutan</title>
</head>
<body>
 <header>
 <h1>Membuat Form</h1>
 </header>
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
   <input id="jk_l" type="radio" name="kelamin" value="L" /><label
   for="jk_l">Laki-laki</label>
    <input id="jk_p" type="radio" name="kelamin" value="P" /><label
    for="jk_p">Perempuan</label>
   </p>
   <p><input type="submit" value="Login"></p>
   </fieldset>
</form>
</body>
</html>
```
![8](https://user-images.githubusercontent.com/56241285/114307930-20f87a00-9b0c-11eb-8bcb-41723326ba81.png)

## LANGKAH 9
### Menambahkan style pada form agar tampilan lebih menarik menggunakan CSS
```
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
![9](https://user-images.githubusercontent.com/56241285/114308153-096dc100-9b0d-11eb-934a-aae2c0402e81.png)

## TUGAS
### Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.
#### Membuat Dropdown Menu dan Listbox dengan multiple selection
```
<!DOCTYPE html>
<html>
<head>
	<title>HTML Lanjutan</title>
</head>
<body>
 
	<style type="text/css">
	html,body{
		padding: 0;
		margin:0;
		font-family: sans-serif;
	}
 
	.menu{
		background-color: #c300ff;
	}
 
	.menu ul {
		list-style-type: none;
		margin: 0;
		padding: 0;
		overflow: hidden;
	}
 
	.menu > ul > li {
		float: left;
	}
 
	
	.menu li a {
		display: inline-block;
		color: white;
		text-align: center;
		padding: 14px 16px;
		text-decoration: none;
	}
 
	.menu li a:hover{
		background-color: #c300ff;
	}
 
	li.dropdown {
		display: inline-block;
	}
 
	.dropdown:hover .isi-dropdown {
		display: block;
	}
 
	.isi-dropdown a:hover {
		color: #fff !important;
	}
 
	.isi-dropdown {
		position: absolute;
		display: none;
		box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
		z-index: 1;
		background-color: #f9f9f9;
	}
 
	.isi-dropdown a {
		color: #3c3c3c !important;
	}
 
	.isi-dropdown a:hover {
		color: #232323 !important;
		background: #f3f3f3 !important;
	}
</style>
 
 
<header class="header">
	<div class="menu">
 
		<ul>
			<li><a href="lab3_tugas.html">Home</a></li>
			<li class="dropdown"><a href="#">DROPDOWN MENU LAB 3 WEB</a>
				<ul class="isi-dropdown">
					<li><a href="lab3_list.html">LAB 3 LIST</a></li>
					<li><a href="lab3_tabel.html">LAB 3 TABEL</a></li>
					<li><a href="lab3_form.html">LAB 3 FORM</a></li>
				</ul>
			</li>
		</ul>
 
	</div>
</header>
 
<br/>
 
<center>
	<h1>Membuat Menu Dropdown dan Listbox</h1>
</center>

<h4>CONTOH LISTBOX</h4>
<form action="proses.php" method="get">
    <p>Pulau Besar
    <select name='pulau Besar' multiple='multiple'>
      <option value='jawa'>jawa</option>
      <option value='sumatra' selected='selected'>sumatra</option>
      <option value='sulawesi'>sulawesi</option>
      <option value='kalimantan'>kalimantan</option>
      <option value='papua'>papua</option>
    </select>
    </p>
    <input type='submit' name='tombol' value='kirim' />
</form>
</body>
</html>
```
![10](https://user-images.githubusercontent.com/56241285/114308971-cfea8500-9b0f-11eb-8210-911949ddb9ee.png)
![11](https://user-images.githubusercontent.com/56241285/114309275-df1e0280-9b10-11eb-9735-56d9550735a8.png)
