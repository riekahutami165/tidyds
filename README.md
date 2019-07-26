
<!-- README.md is generated from README.Rmd. Please edit that file -->

# Fundamental Tidy Data Science in R

## Prosedur

1.  Klik tombol **Fork** pada bagian kanan atas
2.  Setelah berhasil silakan klik tombol **Clone or download** (tombol
    berwarna hijau pada bagian kanan)
3.  Pilih prosedur HTTPS dan salin tautan URL yang disediakan
4.  Buka RStudio Anda dan kemudian pilih menu **File – New Project**
5.  Pilih opsi **Version Control - Git**
6.  Tempelkan tautan yang telah disalin serta sesuaikan lokasi direktori
    sesuai keinginan Anda
7.  Klik tombol **Create Project** untuk mengunduh dan membuka
    repositori ini di RStudio Anda
8.  Lakukan konfigurasi git dengan cara klik menu **Tools – Shell** dan
    jalankan baris kode berikut:

<!-- end list -->

``` bash
git config --global user.email "Email Anda"
git config --global user.name "Nama Anda"
```

9.  Pelajari dan kerjakan latihan soal pada modul yang tersimpan dalam
    subdirektori “vignettes”. Setelah berhasil menyelesaikan suatu modul
    jangan lupa untuk klik tombol **Knit**
10. Setiap selesai mengerjakan modul atau melakukan perubahan Anda
    diminta untuk membuat “git commit”. Caranya adalah klik tab **Git**
    pada **Environment Pane**, berikan tanda centang pada kolom “Staged”
    untuk berkas yang Anda tambahkan atau ubah, klik submenu **Commit**,
    isilah “Commit message” dan kemudian klik tombol **Commit**.
    Sekarang perubahan yang Anda lakukan terlah terekam oleh git
11. Anda dapat mengunggah hasil pekerjaan tersebut secara daring ke
    repositori GitHub dengan cara klik tombol **Push**

## Persiapan

Jalankan baris kode berikut untuk mempersiapkan paket-paket yang akan
digunakan selama pelatihan:

``` r
install.packages("devtools")
devtools::install_deps()
devtools::load_all()
tidyds::check_deps()
```

## Struktur direktori

Repositori ini tersusun atas subdirektori, berkas, dan dokumen sebagai
berikut:

    #> .
    #> ├── data
    #> │   ├── un_smp_lm.rda
    #> │   ├── un_smp_recipe.rda
    #> │   └── un_smp_rf.rda
    #> ├── data-raw
    #> │   ├── anggaran-dinkes-2013.csv
    #> │   ├── anggaran-dinkes-2014.csv
    #> │   ├── anggaran-dinkes-2015.csv
    #> │   ├── anggaran-dinkes-2016.csv
    #> │   ├── anggaran-dinkes-2017.csv
    #> │   ├── anggaran-dinkes-2018.csv
    #> │   ├── content_dev.R
    #> │   ├── Dago.csv
    #> │   ├── Gedebage.csv
    #> │   ├── Pajajaran.csv
    #> │   ├── prep-datasets.R
    #> │   ├── roster.xlsx
    #> │   ├── sherlock.csv
    #> │   ├── udara_bandung.csv
    #> │   ├── udara_bandung.xlsx
    #> │   ├── Ujungberung.csv
    #> │   └── un_smp.csv
    #> ├── DESCRIPTION
    #> ├── inst
    #> │   ├── aq
    #> │   │   ├── global.R
    #> │   │   ├── server.R
    #> │   │   └── ui.R
    #> │   └── ipa
    #> │       ├── global.R
    #> │       ├── server.R
    #> │       └── ui.R
    #> ├── LICENSE
    #> ├── man
    #> │   ├── check_deps.Rd
    #> │   ├── figures
    #> │   │   └── README-pressure-1.png
    #> │   ├── run_aq.Rd
    #> │   └── run_ipa.Rd
    #> ├── NAMESPACE
    #> ├── R
    #> │   ├── check-deps.R
    #> │   ├── run-aq.R
    #> │   └── run-ipa.R
    #> ├── README.md
    #> ├── README.Rmd
    #> ├── tidyds.Rproj
    #> └── vignettes
    #>     ├── m1_essentials-ans.Rmd
    #>     ├── m1_essentials.Rmd
    #>     ├── m2_data-import-ans.Rmd
    #>     ├── m2_data-import.Rmd
    #>     ├── m3_tidy-data-carpentry-ans.Rmd
    #>     ├── m3_tidy-data-carpentry.Rmd
    #>     ├── m4_data-visualisation-ans.Rmd
    #>     ├── m4_data-visualisation.Rmd
    #>     ├── m5_modeling-1-ans.Rmd
    #>     ├── m5_modeling-1.Rmd
    #>     ├── m6_modeling-2-ans.Rmd
    #>     ├── m6_modeling-2.Rmd
    #>     ├── m7_shiny-1-ans.Rmd
    #>     ├── m7_shiny-1.Rmd
    #>     ├── m8_shiny-2-ans.Rmd
    #>     └── m8_shiny-2.Rmd
    #> 
    #> 9 directories, 55 files
