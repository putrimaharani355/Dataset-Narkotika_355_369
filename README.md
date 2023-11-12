# Dataset-Narkotika_355_369

### Scraping Putusan Pidana Khusus
Scraping Data Pengadilan Negeri Jombang Mengenai Pidana Khusus tentang Narkotika dan Psikotropika tahun 2023.

### Dataset
Dataset yang kami gunakan untuk scraping ini adalah 'Pengadilan Negeri Jombang' mengenai 'Pidana Khusus' tentang 'Narkotika dan Psikotropika' tahun 2023. Dimana hasil scraping tersebut berjumlah 168 data. Dataset bisa dilihat [here](https://drive.google.com/drive/folders/1Lbn3_6uAaz0Ppvz1Pr47l7j4BfuV085Q?usp=sharing).

<details>
<summary>URL Scraping</summary>
https://putusan3.mahkamahagung.go.id/search.html?q=&jenis_doc=putusan&cat=3c40e48bbab311301a21c445b3c7fe57&jd=AMAR_LAINNYA&tp=0&court=098188PN317+++++++++++++++++++++&t_put=2023&t_reg=&t_upl=&t_pr=
  
Output Hasil scraping [here](https://drive.google.com/drive/folders/1-09WtL_h_GGngG9gtxN9tlE8-OVzcJAF?usp=sharing)
</details>

### Ekstrak Barang Bukti
Pada file ini kami melakukan ekstrak data hasil scraping dalam bentuk format '.csv', dan kami juga melakukan preprocessing pada file tersebut.
<details>
<summary>Preprocessing</summary>
<summary>Mengupload file 'putusan_ma__2023-11-11 (1).csv'</summary>
<summary>Mengembalikan jumlah nilai NaN di semua kolom pandas DataFrame dengan Python 'df.isna().sum()'</summary>
<summary>Menghapus baris/kolom tertentu 'columns_to_drop'</summary>
</details>
<details>
<summary>Extract</summary>
<summary>Fungsi untuk ekstraksi kalimat dengan kata kunci 'def extract_sentence_with_keyword(text, keyword):'</summary>
<summary>Menambahkan kolom baru ke DataFrame '] = df['catatan_amar'].apply(lambda x: extract_sentence_with_keyword(x, "barang bukti berupa"))' </summary>
<summary>Menyimpan DataFrame ke file CSV baru 'output_csv = 'output_with_barang_bukti.csv'
df.to_csv(output_csv, index=False)'</summary>
<summary>Menampilkan hasil file CSV dengan DataFrame 'df'</summary>
