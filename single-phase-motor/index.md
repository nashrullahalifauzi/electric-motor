---
lang: id-ID
dir: ltr
title: "Motor Satu Fasa: Definisi, Formulasi, dan Prinsip Kerja Gulung Ulang Kumparan"
author: Nashrullah Ali Fauzi
date: \today
#citeproc: true
#cite-method: citeproc
#csl: /home/nf/git/nurbaitifitriyani/film-adaptation/12-bibliography/csl/mla/modern-language-association.csl
#bibliography: /home/nf/git/nurbaitifitriyani/film-adaptation/12-bibliography/bib/film-adaptation-better-biblatex.bib
#suppress-bibliography: false
#link-citations: true
#color-links: true
#linkcolor: black
#urlcolor: black
#citecolor: black
endnote: false
notes-after-punctuation: false
colorlinks: true
toccolor: black
filecolor: black
hyperrefoptions:
- linktoc=all
- pdfwindowui
- pdfpagemode=FullScreen
indent: true
toc-title: 'Daftar Isi'
toc: true
toc_depth: 6
lof: false
lot: false
numbersections: true
secnumdepth: 6
number-sections: true
subparagraph: 'yes'
fontsize: 12pt
linestretch: 1.5
strip-comments: true
xnos-number-by-section: true
mainfont: "Merriweather"
sansfont: "Raleway"
monofont: "IBM Plex Mono"
documentclass: article
classoption: [notitlepage, onecolumn]
geometry: [a4paper, bindingoffset=0mm, inner=30mm, outer=30mm, top=30mm, bottom=30mm]
---

# Pengantar

# Introduksi: Motor Satu Fasa

Berikut adalah penjelasan terperinci mengenai definisi, komponen, dan cara kerja motor listrik satu fasa.

## Definisi

Motor satu fasa adalah jenis motor listrik yang dirancang untuk beroperasi menggunakan sumber daya listrik arus bolak-balik (AC) satu fasa. Ini adalah jenis motor yang paling umum ditemukan dalam peralatan rumah tangga (seperti kipas angin, pompa air, lemari es, mesin cuci) dan peralatan komersial serta industri skala kecil.

Ciri utama motor satu fasa adalah ia **tidak dapat memulai putarannya sendiri** (*not self-starting*) jika hanya mengandalkan satu belitan stator yang dialiri arus AC satu fasa. Hal ini karena medan magnet yang dihasilkan oleh arus AC satu fasa pada satu belitan bersifat **pulsating** (berdenyut maju-mundur pada satu sumbu), bukan **rotating** (berputar) seperti pada motor tiga fasa. Medan magnet pulsating ini tidak cukup untuk menghasilkan torsi awal (starting torque) untuk menggerakkan rotor dari keadaan diam. Oleh karena itu, motor satu fasa memerlukan desain atau komponen tambahan untuk menciptakan kondisi medan magnet yang seolah-olah berputar pada saat start.

## Komponen Utama

Komponen utama motor induksi satu fasa umumnya meliputi:

1.  **Stator:**
    * **Fungsi:** Bagian motor yang diam, berfungsi sebagai tempat dihasilkannya medan magnet utama.
    * **Struktur:**
        * **Inti Stator (Stator Core):** Terbuat dari lembaran-lembaran besi lunak atau baja silikon yang dilaminasi (dipress menjadi satu) untuk mengurangi rugi-rugi akibat arus eddy (*eddy current losses*). Inti ini memiliki alur-alur (slots) di bagian dalamnya.
        * **Belitan Stator (Stator Winding):** Kumparan kawat tembaga beremail yang dimasukkan ke dalam alur-alur inti stator. Pada motor satu fasa (selain tipe *shaded pole*), umumnya terdapat dua set belitan:
            * **Belitan Utama (Main Winding / Run Winding):** Belitan dengan jumlah lilitan lebih banyak dan diameter kawat lebih besar (resistansi lebih rendah, reaktansi lebih tinggi). Belitan ini tetap terhubung ke sumber listrik selama motor beroperasi.
            * **Belitan Bantu (Auxiliary Winding / Start Winding):** Belitan dengan jumlah lilitan lebih sedikit dan diameter kawat lebih kecil (resistansi lebih tinggi, reaktansi lebih rendah). Ditempatkan secara fisik berbeda (biasanya 90 derajat listrik) dari belitan utama. Fungsinya hanya untuk membantu proses start. Pada banyak jenis motor, belitan ini akan diputus dari rangkaian setelah motor mencapai kecepatan tertentu.

2.  **Rotor:**
    * **Fungsi:** Bagian motor yang berputar, menghasilkan gerakan mekanis.
    * **Struktur:** Jenis rotor yang paling umum digunakan pada motor induksi satu fasa adalah **rotor sangkar tupai (Squirrel Cage Rotor)**.
        * **Inti Rotor (Rotor Core):** Juga terbuat dari laminasi besi untuk mengurangi rugi arus eddy, memiliki alur-alur.
        * **Batang Konduktor (Rotor Bars):** Batang-batang konduktor (biasanya aluminium atau tembaga) yang diletakkan di dalam alur inti rotor.
        * **Cincin Hubung Singkat (End Rings):** Kedua ujung batang konduktor dihubung singkat oleh cincin konduktif. Struktur ini menyerupai sangkar tupai. Rotor jenis ini tidak memerlukan suplai listrik eksternal.

3.  **Mekanisme Starting:**
    * **Fungsi:** Komponen atau metode yang digunakan untuk menghasilkan torsi awal agar motor dapat mulai berputar.
    * **Jenis Umum:**
        * **Saklar Sentrifugal (Centrifugal Switch):** Perangkat mekanis yang terpasang pada poros rotor. Ketika motor mencapai sekitar 75-80% dari kecepatan nominalnya, gaya sentrifugal akan menyebabkan saklar ini membuka kontak listriknya. Fungsinya adalah untuk memutuskan hubungan belitan bantu (dan/atau kapasitor start) dari sumber listrik setelah motor berhasil start.
        * **Kapasitor (Capacitor):** Digunakan pada jenis motor kapasitor. Bisa berupa:
            * *Kapasitor Start (Start Capacitor):* Dihubungkan seri dengan belitan bantu untuk menciptakan beda fasa arus yang besar saat start, menghasilkan torsi start yang tinggi. Biasanya diputus oleh saklar sentrifugal.
            * *Kapasitor Run (Run Capacitor):* Dihubungkan seri dengan belitan bantu (atau belitan khusus) dan tetap terhubung selama motor beroperasi. Berfungsi untuk memperbaiki faktor daya dan efisiensi motor. Nilai kapasitansinya lebih kecil daripada kapasitor start.
            * Beberapa motor menggunakan keduanya (*Capacitor-Start Capacitor-Run*).
        * **Metode Kutub Bayangan (Shaded Pole):** Pada motor jenis *shaded pole*, sebagian kecil dari setiap kutub stator dilingkari oleh cincin tembaga hubung singkat (*shading coil*). Ini menyebabkan fluks magnet di area yang dilingkari tertinggal (lag) dibandingkan fluks di area utama, menciptakan medan magnet lemah yang bergeser dan cukup untuk memulai putaran pada aplikasi torsi rendah (misalnya kipas angin kecil).

4.  **Bearing (Bantalan):**
    * **Fungsi:** Mendukung poros rotor di kedua ujungnya, memungkinkan rotor berputar dengan bebas dan gesekan minimal, serta menjaga celah udara (air gap) antara rotor dan stator tetap konstan.

5.  **Rumah Motor (Enclosure / Housing):**
    * **Fungsi:** Melindungi komponen internal motor dari debu, kelembaban, dan benturan fisik. Juga berfungsi sebagai struktur penopang stator dan bearing, serta membantu pembuangan panas.

## Prinsip Kerja Motor Satu Fasa

Prinsip kerja motor induksi satu fasa (misalnya jenis kapasitor start) dapat dijelaskan sebagai berikut:

1.  **Saat Start (Starting):**
    * Ketika sumber tegangan AC satu fasa diberikan, arus mengalir ke belitan utama dan belitan bantu (yang terhubung seri dengan kapasitor start dan kontak saklar sentrifugal yang normalnya tertutup saat diam).
    * Karena adanya kapasitor pada rangkaian belitan bantu, arus yang mengalir pada belitan bantu ($I_{aux}$) akan **mendahului (lead)** tegangan suplai. Sementara itu, arus pada belitan utama ($I_{main}$) yang bersifat induktif akan **tertinggal (lag)** dari tegangan suplai.
    * Akibatnya, tercipta beda fasa waktu antara $I_{main}$ dan $I_{aux}$. Kedua arus ini menghasilkan medan magnet masing-masing ($F_{main}$ dan $F_{aux}$) yang juga berbeda fasa.
    * Kombinasi kedua medan magnet yang berbeda fasa dan berbeda posisi fisik (90 derajat listrik) ini menghasilkan medan magnet resultan yang **berputar** (atau setidaknya mendekati berputar) di dalam celah udara.

2.  **Induksi pada Rotor:**
    * Medan magnet putar dari stator ini memotong batang-batang konduktor pada rotor sangkar tupai.
    * Sesuai hukum induksi Faraday, GGL (Gaya Gerak Listrik) terinduksi pada batang rotor.
    * Karena batang rotor dihubung singkat oleh cincin ujung, GGL ini menyebabkan arus mengalir pada batang rotor.

3.  **Menghasilkan Torsi:**
    * Arus yang mengalir pada rotor ini berinteraksi dengan medan magnet putar stator (sesuai hukum gaya Lorentz).
    * Interaksi ini menghasilkan gaya pada batang-batang rotor yang arahnya sedemikian rupa sehingga menciptakan **torsi** (momen putar) pada rotor.
    * Torsi ini disebut torsi induksi, dan inilah yang menyebabkan rotor mulai berputar mengikuti arah medan magnet putar stator.

4.  **Saat Beroperasi Normal (Running):**
    * Ketika kecepatan rotor meningkat hingga mencapai sekitar 75-80% kecepatan sinkronnya, gaya sentrifugal pada mekanisme saklar sentrifugal menjadi cukup kuat untuk membuka kontaknya.
    * Pembukaan saklar ini akan memutuskan aliran arus ke belitan bantu dan kapasitor start.
    * Motor kemudian terus berputar hanya dengan daya dari belitan utama. Medan magnet yang dihasilkan oleh belitan utama saja kini bersifat pulsating, namun karena rotor sudah berputar, interaksi antara medan pulsating ini dengan arus induksi di rotor cukup untuk menghasilkan torsi yang menjaga putaran motor dan mengatasi beban (selama beban tidak berlebih). Rotor berputar pada kecepatan sedikit di bawah kecepatan sinkron medan magnet (disebut slip).

Pada jenis motor lain seperti PSC (Permanent Split Capacitor), kapasitor dan belitan bantu tetap terhubung selama operasi untuk meningkatkan performa dan efisiensi. Pada motor *shaded pole*, medan magnet bergeser yang lemah sudah cukup untuk start dan operasi pada beban sangat ringan.

Tentu, mari kita jelaskan secara terperinci tentang motor satu fasa yang digunakan untuk pompa air.

# Bab I: Pompa Air Motor Satu Fasa

Motor satu fasa untuk pompa air adalah motor listrik AC satu fasa yang dirancang khusus untuk menggerakkan mekanisme pompa air. Pompa air memerlukan motor yang dapat memberikan torsi yang cukup untuk memulai aliran air dan mempertahankannya selama operasi. Motor satu fasa dipilih untuk aplikasi ini karena ketersediaan sumber listrik satu fasa di sebagian besar lokasi perumahan dan komersial kecil, serta biaya yang relatif lebih rendah dibandingkan motor tiga fasa.

## Komponen Utama

Komponen motor satu fasa pada pompa air pada dasarnya sama dengan motor satu fasa pada umumnya, namun ada beberapa pertimbangan spesifik terkait aplikasi pompa air:

1.  **Stator:** Bagian yang diam dengan inti besi laminasi dan alur untuk kumparan. Pada motor pompa air, stator memiliki:
    * **Kumparan Utama (Running Winding):** Berukuran lebih besar dan didesain untuk operasi kontinu setelah motor mencapai kecepatan kerja.
    * **Kumparan Bantu (Starting Winding):** Berukuran lebih kecil, memiliki resistansi yang lebih tinggi, dan berfungsi khusus untuk memberikan torsi awal saat motor dihidupkan. Kumparan ini biasanya terpisah secara elektrik sebesar 90 derajat dari kumparan utama.

2.  **Rotor (Squirrel Cage Rotor):** Bagian yang berputar, terdiri dari inti besi laminasi dengan batang-batang konduktor yang dihubung singkat. Rotor ini dirancang untuk menahan beban puntir (torsi) yang diperlukan untuk memutar impeler pompa.

3.  **Alat Bantu Start:** Ini adalah komponen krusial pada motor pompa air satu fasa agar dapat memulai putaran. Jenis motor satu fasa yang umum digunakan untuk pompa air biasanya menggunakan kapasitor sebagai alat bantu start:
    * **Motor Kapasitor Start - Induksi Run (CSIR):** Menggunakan kapasitor elektrolitik yang terhubung seri dengan kumparan bantu dan saklar sentrifugal. Kapasitor ini memberikan torsi start yang tinggi untuk mengatasi inersia awal pompa dan kolom air. Setelah motor mencapai kecepatan tertentu, saklar sentrifugal memutuskan kapasitor dan kumparan bantu.
    * **Motor Kapasitor Start - Kapasitor Run (CSCR):** Menggunakan dua kapasitor: kapasitor start (elektrolitik) dan kapasitor run (minyak). Kapasitor start terhubung seri dengan kumparan bantu dan saklar sentrifugal seperti pada motor CSIR. Kapasitor run terhubung secara permanen seri dengan kumparan bantu. Kombinasi ini memberikan torsi start yang tinggi dan meningkatkan efisiensi serta faktor daya selama operasi berjalan. Jenis ini sering digunakan untuk pompa air dengan daya yang lebih besar.
    * **Motor Permanent Split Capacitor (PSC):** Hanya menggunakan satu kapasitor (biasanya jenis minyak) yang terhubung secara permanen seri dengan kumparan bantu. Motor jenis ini memiliki torsi start yang lebih rendah dibandingkan motor CSIR atau CSCR, sehingga lebih cocok untuk pompa dengan kebutuhan torsi start yang tidak terlalu tinggi.

4.  **Saklar Sentrifugal (Centrifugal Switch):** Umum ditemukan pada motor pompa air jenis kapasitor start. Saklar ini terpasang pada poros rotor dan berfungsi secara otomatis melepaskan kumparan bantu (beserta kapasitor start jika ada) dari rangkaian listrik saat kecepatan rotor mencapai sekitar 70-80% dari kecepatan nominal. Ini penting karena kumparan bantu dan kapasitor start tidak didesain untuk beroperasi secara terus-menerus.

5.  **Poros (Shaft):** Menghubungkan rotor motor dengan impeler pompa. Poros ini harus kuat untuk menahan torsi putar dan gaya aksial/radial dari pompa.

6.  **Rumah Motor (Motor Housing):** Struktur luar yang melindungi komponen internal motor dari lingkungan. Untuk aplikasi pompa air, rumah motor seringkali didesain untuk tahan terhadap kelembaban dan percikan air (rating IP yang sesuai).

7.  **Kipas Pendingin (Cooling Fan):** Terpasang pada poros motor untuk membantu mendinginkan motor selama operasi, mencegah panas berlebih.

8.  **Bearing (Bantalan):** Mendukung poros rotor dan memungkinkan putaran yang lancar dengan gesekan minimal.

### Tahap-Tahap Motor Pompa Air Hidup

Cara kerja motor satu fasa pada pompa air melibatkan dua tahap utama: tahap start dan tahap operasi berjalan.

1.  **Tahap Start:**
    * Ketika motor dihubungkan ke sumber listrik satu fasa, arus mengalir melalui kumparan utama dan kumparan bantu (melalui alat bantu start seperti kapasitor).
    * Adanya alat bantu start (kapasitor) menciptakan perbedaan fasa antara arus yang mengalir pada kumparan utama dan kumparan bantu. Perbedaan fasa arus ini menghasilkan dua medan magnet berdenyut yang tidak sefasa dan terpisah secara spasial (kumparan utama dan bantu terpisah 90 derajat).
    * Kombinasi dua medan magnet berdenyut yang berbeda fasa ini menghasilkan medan magnet gabungan yang berputar (atau setidaknya medan magnet elips yang kuat) di celah udara stator.
    * Medan magnet putar ini memotong batang-batang konduktor pada rotor sangkar tupai, menginduksi tegangan dan arus pada rotor.
    * Interaksi antara medan magnet stator yang berputar dan medan magnet yang dihasilkan oleh arus rotor menghasilkan torsi putar awal (starting torque). Torsi ini harus cukup besar untuk mengatasi inersia rotor, impeler pompa, dan gesekan awal air.
    * Rotor mulai berputar mengikuti arah putaran medan magnet stator.

2.  **Tahap Operasi Berjalan (Running):**
    * Saat kecepatan rotor meningkat dan mencapai sekitar 70-80% dari kecepatan sinkron, saklar sentrifugal (jika ada) akan terbuka dan memutuskan hubungan kumparan bantu (beserta kapasitor start pada motor CSIR/CSCR) dari sumber listrik.
    * Motor kemudian beroperasi hanya dengan kumparan utama yang terhubung langsung ke sumber listrik satu fasa.
    * Pada tahap ini, medan magnet yang dihasilkan oleh kumparan utama bersifat berdenyut. Namun, karena rotor sudah berputar, ada efek "medan silang" yang terinduksi pada rotor yang bergerak. Interaksi antara medan magnet berdenyut stator dan medan magnet terinduksi pada rotor yang berputar inilah yang mempertahankan torsi dan menjaga motor tetap berputar.
    * Pada motor PSC dan CSCR, kumparan bantu (dengan kapasitor run pada CSCR) tetap terhubung selama operasi berjalan untuk meningkatkan efisiensi, faktor daya, dan memberikan karakteristik torsi yang lebih baik.
    * Kecepatan rotor selama operasi berjalan akan sedikit lebih rendah dari kecepatan sinkron medan magnet stator. Perbedaan ini (slip) diperlukan untuk menginduksi arus pada rotor.

Motor satu fasa untuk pompa air, khususnya jenis kapasitor start atau kapasitor start-run, dipilih karena kemampuannya memberikan torsi start yang memadai untuk aplikasi pompa. Desain komponen seperti motor housing juga disesuaikan untuk lingkungan kerja pompa air yang seringkali lembab.

## Stator Motor Satu Fasa Pompa Air: Kumparan Utama dan Kumparan Bantu

Stator pada motor satu fasa pompa air adalah bagian diam yang berfungsi menghasilkan medan magnet. Medan magnet ini kemudian berinteraksi dengan rotor untuk menghasilkan putaran. Stator terdiri dari inti besi berlaminasi (untuk mengurangi kerugian arus eddy) yang memiliki sejumlah alur atau slot di permukaan bagian dalamnya. Di dalam alur-alur inilah kumparan kawat tembaga ditempatkan.

Pada motor satu fasa, stator memiliki dua jenis kumparan utama:

1.  **Kumparan Utama (Main Winding / Running Winding):** Kumparan ini didesain untuk membawa sebagian besar arus selama operasi normal motor dan bertanggung jawab untuk mempertahankan putaran motor. Ciri-ciri kumparan utama meliputi:
    * **Jumlah Lilitan:** Relatif lebih banyak dibandingkan kumparan bantu.
    * **Diameter Kawat:** Menggunakan kawat tembaga dengan diameter yang lebih besar, sehingga memiliki resistansi yang lebih rendah.
    * **Tata Letak (Pitch):** Biasanya memiliki langkah kumparan (coil pitch) yang lebih besar, mendekati 180 derajat listrik atau satu kutub penuh, meskipun bisa sedikit diperpendek untuk mengurangi harmonisa.
    * **Penempatan:** Ditempatkan pada alur-alur yang tersebar di sekeliling stator.

2.  **Kumparan Bantu (Auxiliary Winding / Starting Winding):** Kumparan ini secara khusus didesain untuk menghasilkan medan magnet yang bergeser fasa pada saat motor mulai berputar (starting). Setelah motor mencapai kecepatan tertentu, kumparan ini biasanya dilepaskan dari rangkaian (pada jenis motor kapasitor start atau fasa belah). Ciri-ciri kumparan bantu meliputi:
    * **Jumlah Lilitan:** Relatif lebih sedikit dibandingkan kumparan utama.
    * **Diameter Kawat:** Menggunakan kawat tembaga dengan diameter yang lebih kecil, sehingga memiliki resistansi yang lebih tinggi.
    * **Tata Letak (Pitch):** Biasanya memiliki langkah kumparan (coil pitch) yang lebih pendek dibandingkan kumparan utama.
    * **Penempatan:** Ditempatkan pada alur-alur yang berjarak 90 derajat listrik dari kumparan utama. Penempatan ini penting untuk menciptakan perbedaan fasa medan magnet yang optimal untuk start.

### Jumlah Lubang Stator (Alur/Slot)

Jumlah lubang atau alur pada stator motor satu fasa bervariasi tergantung pada ukuran motor (daya), jumlah kutub (poles), dan desain spesifik pabrikan. Namun, ada prinsip dasar terkait hubungan antara jumlah alur dan jumlah kutub.

Jumlah alur stator ($Q_s$) biasanya merupakan kelipatan genap dan umumnya cukup untuk menampung kumparan utama dan bantu secara terdistribusi untuk membentuk jumlah kutub yang diinginkan (misalnya, 2 kutub, 4 kutub). Motor pompa air umum biasanya adalah motor 2-kutub atau 4-kutub.

Beberapa contoh jumlah alur yang umum:

* Untuk motor 2 kutub atau 4 kutub, jumlah alur bisa berupa 12, 16, 24, 32, atau 36. Angka-angka ini sering dipilih karena memudahkan dalam mendistribusikan kumparan utama dan bantu secara simetris dan berjarak 90 derajat listrik.

Jumlah alur per kutub per fasa ($q$) adalah faktor penting dalam desain belitan:
$q = Q_s / (2 \times \text{jumlah kutub} \times \text{jumlah fasa})$

Karena ini motor satu fasa dengan dua kumparan yang diperlakukan seperti dua fasa saat start (meskipun hanya satu sumber fasa), perhitungannya disesuaikan. Penempatan kumparan utama dan bantu pada alur-alur ini bertujuan untuk menciptakan distribusi medan magnet yang mendekati sinusoidal di celah udara.

### Alur dan Jalur Kawat untuk Kumparan Utama dan Kumparan Bantu**

Kumparan utama dan kumparan bantu ditempatkan pada alur-alur stator dengan pola tertentu.

* **Penempatan Kumparan Utama:** Lilitan kumparan utama ditempatkan pada alur-alur yang membentuk kelompok kumparan (coil group). Setiap kelompok kumparan mencakup beberapa alur dan memiliki polaritas (Utara atau Selatan) ketika dialiri arus. Jumlah kelompok kumparan utama sama dengan jumlah kutub motor. Setiap kelompok kumparan utama ini tersebar di beberapa alur untuk mendapatkan distribusi medan magnet yang lebih baik.

* **Penempatan Kumparan Bantu:** Kumparan bantu ditempatkan pada alur-alur yang berada pada posisi 90 derajat listrik dari pusat setiap kelompok kumparan utama. Seperti kumparan utama, kumparan bantu juga disusun dalam kelompok kumparan. Penempatan ini memungkinkan medan magnet yang dihasilkan oleh kumparan bantu memiliki perbedaan fasa spasial 90 derajat dengan medan magnet utama, yang, dikombinasikan dengan perbedaan fasa arus (berkat kapasitor atau resistansi yang berbeda), akan menghasilkan medan magnet putar.

### Contoh Tata Letak Sederhana (Motor 4 Kutub dengan 24 Alur):

Untuk motor 4 kutub dengan 24 alur, akan ada 4 kutub Utara dan 4 kutub Selatan (secara bergantian) yang dibentuk oleh kumparan utama. Total alur per kutub adalah $24 / 4 = 6$ alur/kutub.

* Jarak 1 kutub listrik adalah $180^\circ$ listrik, yang setara dengan $24/4 \times 180^\circ / 180^\circ = 6$ alur mekanik.
* Jarak 90 derajat listrik adalah $90^\circ / 180^\circ \times 6$ alur = 3 alur mekanik.

Jika kumparan utama dimulai pada alur 1, maka kelompok kumparan utama akan menduduki alur-alur dengan pola tertentu untuk membentuk 4 kutub. Kumparan bantu akan ditempatkan pada alur yang berjarak 3 alur mekanik dari alur awal kumparan utama, misalnya dimulai pada alur 1 + 3 = alur 4, dan juga tersebar dalam kelompok untuk membentuk 4 kutub bantu yang bergeser 90 derajat listrik.

Setiap alur dapat menampung sisi-sisi dari beberapa kumparan yang berbeda (lap winding atau wave winding), membentuk pola belitan yang kompleks untuk mencapai jumlah lilitan dan distribusi yang diinginkan untuk kumparan utama dan bantu. Kawat tembaga yang telah dilapisi insulasi dimasukkan ke dalam alur-alur ini, dan di ujung stator, lilitan-lilitan ini saling dihubungkan sesuai dengan diagram pengawatan motor untuk membentuk kumparan utama dan bantu dengan jumlah kutub yang benar.

Ringkasnya, jumlah lubang stator, alur, dan tata letak belitan kawat tembaga untuk kumparan utama dan bantu dirancang secara cermat untuk:
1.  Menciptakan medan magnet yang optimal.
2.  Menghasilkan torsi start yang cukup (dengan bantuan kumparan bantu).
3.  Memastikan operasi motor yang efisien dan andal untuk menggerakkan beban pompa air.

## Rotor Motor Satu Fasa Pompa Air

Rotor adalah bagian motor yang berputar dan berfungsi mengubah energi listrik yang diinduksi menjadi energi mekanik berupa gerakan rotasi pada poros. Pada motor induksi satu fasa, termasuk yang digunakan untuk pompa air, jenis rotor yang paling umum adalah **rotor sangkar tupai (squirrel cage rotor)**. Dinamakan demikian karena konstruksinya menyerupai sangkar tupai.

Berikut adalah penjelasan terperinci mengenai rotor sangkar tupai pada motor satu fasa pompa air:

### Konstruksi Rotor Sangkar Tupai

1.  **Inti Rotor:** Terbuat dari tumpukan laminasi baja silikon tipis. Laminasi ini bertujuan untuk mengurangi kerugian akibat arus eddy yang terinduksi pada inti rotor. Laminasi ini disusun dan diklem menjadi satu silinder yang kokoh. Permukaan luar inti rotor memiliki alur-alur memanjang yang sejajar atau sedikit miring (skewed) terhadap poros.

2.  **Batang Konduktor Rotor (Rotor Bars):** Batang-batang ini terbuat dari bahan konduktor listrik, biasanya aluminium atau tembaga. Batang-batang ini ditempatkan di dalam alur-alur pada permukaan inti rotor. Untuk motor berukuran kecil hingga menengah seperti pada pompa air rumah tangga, batang konduktor ini seringkali dicetak (die-cast) menggunakan aluminium cair yang dituangkan langsung ke dalam alur laminasi rotor, membentuk batang konduktor dan cincin ujung secara simultan. Untuk motor yang lebih besar atau aplikasi yang lebih menuntut, batang konduktor tembaga bisa digunakan dan kemudian dihubungkan ke cincin ujung melalui proses brazing atau pengelasan. Batang konduktor ini tidak memiliki insulasi satu sama lain.

3.  **Cincin Ujung (End Rings):** Dua buah cincin logam (aluminium atau tembaga) yang ditempatkan di kedua ujung inti rotor. Cincin ujung ini secara permanen menghubungkan ujung-ujung semua batang konduktor rotor, sehingga membentuk rangkaian listrik tertutup yang menyerupai sangkar. Fungsi utama cincin ujung adalah untuk menghubung singkat semua batang konduktor, memungkinkan arus mengalir di dalamnya ketika medan magnet stator menginduksi tegangan.

4.  **Poros Rotor (Rotor Shaft):** Batang logam yang kokoh yang melewati pusat inti rotor dan terhubung erat dengannya. Poros inilah yang terhubung ke beban mekanik, yaitu impeler pompa air. Poros ini ditopang oleh bantalan (bearing) pada kedua ujungnya, memungkinkan rotor berputar dengan bebas di dalam stator.

5.  **Kipas Rotor (Cooling Fan):** Pada banyak motor, kipas pendingin kecil terpasang pada poros rotor di salah satu ujungnya. Kipas ini ikut berputar bersama rotor dan berfungsi mengalirkan udara untuk membantu mendinginkan motor.

### Kemiringan (Skewing) Alur Rotor

Alur pada rotor sangkar tupai seringkali dibuat sedikit miring (skewed) terhadap poros motor. Kemiringan ini memiliki beberapa keuntungan:

* **Mengurangi Kebisingan dan Getaran:** Membantu meratakan torsi yang dihasilkan, sehingga mengurangi dengungan (humming) dan getaran saat motor beroperasi.
* **Mencegah Magnetic Locking (Cogging):** Mencegah gigi-gigi stator dan rotor saling menarik dan terkunci saat motor hendak mulai berputar, yang dapat menyebabkan kegagalan start.
* **Meningkatkan Torsi Awal:** Pada beberapa desain, kemiringan ini dapat sedikit meningkatkan torsi awal.

### Cara Kerja Rotor dalam Konteks Pompa Air

Cara kerja rotor sangkar tupai pada motor satu fasa pompa air sangat erat kaitannya dengan medan magnet stator dan prinsip induksi elektromagnetik:

1.  **Induksi Tegangan:** Ketika motor dihidupkan (menggunakan mekanisme start yang menciptakan medan magnet putar di stator), medan magnet putar ini bergerak melintasi celah udara dan memotong batang-batang konduktor pada rotor yang awalnya diam. Sesuai dengan Hukum Faraday tentang induksi elektromagnetik, pergerakan relatif antara medan magnet dan konduktor menginduksi tegangan (GGL) pada setiap batang konduktor rotor.

2.  **Aliran Arus Rotor:** Karena batang-batang konduktor rotor dihubung singkat oleh cincin ujung, tegangan terinduksi ini menyebabkan arus listrik mengalir melalui batang-batang konduktor dan cincin ujung, membentuk rangkaian tertutup. Frekuensi arus rotor ini pada awalnya sama dengan frekuensi suplai stator saat rotor diam.

3.  **Pembentukan Medan Magnet Rotor:** Arus yang mengalir pada batang-batang konduktor rotor ini juga menghasilkan medan magnet di sekitar rotor. Medan magnet rotor ini selalu berusaha melawan perubahan fluks yang menyebabkannya (sesuai Hukum Lenz). Karena penyebabnya adalah medan magnet stator yang berputar, medan magnet rotor akan berusaha "mengejar" putaran medan magnet stator.

4.  **Produksi Torsi:** Interaksi antara medan magnet stator yang berputar dan medan magnet yang dihasilkan oleh arus terinduksi pada rotor menciptakan gaya pada setiap batang konduktor rotor. Gaya-gaya ini secara kolektif menghasilkan torsi putar pada poros rotor. Torsi inilah yang menggerakkan rotor dan porosnya, yang kemudian memutar impeler pompa air.

5.  **Slip:** Rotor tidak pernah berputar pada kecepatan yang sama persis dengan kecepatan medan magnet stator (kecepatan sinkron). Selalu ada perbedaan kecepatan yang disebut "slip". Slip ini penting karena tanpa slip, tidak akan ada pergerakan relatif antara medan magnet stator dan rotor, sehingga tidak ada tegangan yang terinduksi, tidak ada arus rotor, dan tidak ada torsi yang dihasilkan. Besar kecilnya slip tergantung pada beban yang ditanggung motor; semakin berat beban pompa air, semakin besar slipnya (kecepatan rotor semakin rendah) agar torsi yang dihasilkan cukup untuk mengatasi beban tersebut.

Dalam aplikasi pompa air, rotor sangkar tupai adalah pilihan yang ideal karena konstruksinya yang sederhana, kokoh, andal, dan memerlukan perawatan minimal. Kemampuannya menghasilkan torsi yang cukup saat berputar, meskipun torsi startnya memerlukan bantuan kumparan bantu dan kapasitor pada motor satu fasa, menjadikannya pilihan yang tepat untuk menggerakkan impeler pompa.

## Kapasitor

Kapasitor, yang juga dikenal sebagai kondensator, adalah komponen elektronik pasif yang berfungsi untuk menyimpan energi dalam medan listrik. Secara struktural, kapasitor paling sederhana terdiri dari dua lempengan konduktor (biasanya pelat logam atau foil) yang diletakkan sejajar dan dipisahkan oleh bahan isolator yang disebut dielektrik. Bahan dielektrik ini bisa berupa kertas, mika, keramik, film plastik, atau elektrolit.

Kemampuan kapasitor untuk menyimpan muatan listrik diukur dengan satuan kapasitansi, yang dinyatakan dalam Farad (F). Nilai kapasitansi dipengaruhi oleh luas permukaan lempengan konduktor, jarak antar lempengan, dan jenis bahan dielektrik yang digunakan.

Prinsip dasar kerja kapasitor adalah sebagai berikut: ketika kapasitor dihubungkan dengan sumber tegangan, muatan listrik akan menumpuk pada lempengan-lempengan konduktor. Salah satu lempengan akan mengumpulkan muatan positif, sementara lempengan lainnya mengumpulkan muatan negatif dengan jumlah yang sama. Muatan ini tersimpan selama ada beda potensial antara kedua lempengan. Bahan dielektrik di antara lempengan mencegah arus listrik mengalir langsung di antara keduanya (dalam kondisi ideal). Kapasitor memiliki kemampuan untuk mengisi (charging) dan mengosongkan (discharging) muatan.

### Prinsip Kerja Kapasitor dalam Pompa Air Motor Satu Fasa

Pada motor satu fasa, kapasitor memainkan peran yang sangat penting, terutama pada saat start. Seperti yang telah dibahas sebelumnya, motor induksi satu fasa tidak memiliki torsi start sendiri karena medan magnet yang dihasilkan oleh kumparan utama stator yang dialiri arus AC satu fasa bersifat berdenyut (pulsating), bukan berputar. Kapasitor digunakan untuk mengatasi masalah ini dengan menciptakan perbedaan fasa arus yang diperlukan untuk menghasilkan medan magnet putar awal.

Berikut adalah prinsip kerja kapasitor dalam konteks motor satu fasa pompa air:

1.  **Penciptaan Perbedaan Fasa Arus:**
    * Motor satu fasa pompa air memiliki dua kumparan di stator: kumparan utama (main winding) dan kumparan bantu (auxiliary winding) yang terpisah secara spasial (biasanya 90 derajat listrik).
    * Kumparan utama didesain memiliki reaktansi induktif yang tinggi dan resistansi rendah. Arus yang mengalir melalui kumparan utama akan tertinggal (lagging) relatif terhadap tegangan suplai karena sifat induktifnya.
    * Kumparan bantu, di sisi lain, didesain memiliki resistansi yang lebih tinggi. Yang terpenting, pada motor kapasitor, sebuah kapasitor dihubungkan secara seri dengan kumparan bantu.
    * Kapasitor memiliki sifat listrik yang berlawanan dengan induktor; kapasitor menyebabkan arus yang mengalir melaluinya mendahului (leading) tegangan.
    * Dengan menempatkan kapasitor seri dengan kumparan bantu, impedansi total dari rangkaian kumparan bantu menjadi dominan kapasitif atau setidaknya memiliki reaktansi total yang berlawanan dengan kumparan utama. Ini menyebabkan arus yang mengalir melalui kumparan bantu memiliki perbedaan fasa yang signifikan (mendekati 90 derajat listrik dalam kondisi ideal) terhadap arus yang mengalir melalui kumparan utama. Arus pada kumparan bantu akan cenderung mendahului arus pada kumparan utama.

2.  **Pembentukan Medan Magnet Putar:**
    * Kedua kumparan (utama dan bantu) ditempatkan pada stator dengan pemisahan spasial 90 derajat listrik.
    * Ketika kedua kumparan ini dialiri arus AC yang memiliki perbedaan fasa waktu (sekitar 90 derajat) dan ditempatkan dengan perbedaan spasial 90 derajat, gabungan medan magnet yang dihasilkannya di celah udara stator akan menjadi medan magnet yang berputar (rotating magnetic field). Medan magnet ini mungkin tidak sepenuhnya melingkar (sempurna seperti pada motor tiga fasa), tetapi cukup elips untuk menghasilkan torsi awal.

3.  **Pembangkitan Torsi Awal:**
    * Medan magnet putar yang dihasilkan oleh interaksi kumparan utama dan bantu (dengan bantuan kapasitor) akan memotong batang-batang konduktor pada rotor sangkar tupai.
    * Seperti yang dijelaskan sebelumnya, ini menginduksi tegangan dan arus pada rotor.
    * Interaksi antara medan magnet stator yang berputar dan medan magnet yang dihasilkan oleh arus rotor menghasilkan torsi putar awal (starting torque) yang diperlukan untuk memulai pergerakan rotor dan menggerakkan pompa air.

4.  **Jenis Kapasitor pada Motor Pompa Air:**
    * **Kapasitor Start:** Didesain untuk memberikan torsi awal yang tinggi. Kapasitor ini biasanya memiliki nilai kapasitansi yang lebih besar dan terbuat dari bahan elektrolitik yang cocok untuk operasi intermiten (singkat saat start). Kapasitor start biasanya dilepas dari rangkaian oleh saklar sentrifugal setelah motor mencapai kecepatan tertentu.
    * **Kapasitor Run:** Didesain untuk beroperasi secara kontinu. Kapasitor ini biasanya memiliki nilai kapasitansi yang lebih kecil dan terbuat dari bahan film (seperti polypropylene) yang lebih tahan lama dan memiliki kerugian daya yang rendah. Kapasitor run membantu meningkatkan efisiensi, faktor daya, dan karakteristik kerja motor selama operasi normal. Motor yang hanya menggunakan kapasitor run disebut motor permanent split capacitor (PSC).
    * **Motor Kapasitor Start-Run:** Menggunakan kombinasi kapasitor start dan kapasitor run untuk mendapatkan torsi start yang tinggi dan kinerja operasi berjalan yang baik.

### Kesimpulan

Kapasitor sangat vital dalam motor satu fasa pompa air. Fungsi utamanya adalah untuk menciptakan perbedaan fasa arus antara kumparan utama dan kumparan bantu pada saat start. Perbedaan fasa arus ini, dikombinasikan dengan penempatan spasial kumparan, menghasilkan medan magnet putar di stator yang mampu menginduksi arus pada rotor dan menghasilkan torsi awal. Tanpa kapasitor (atau mekanisme start lainnya), motor satu fasa tidak akan dapat memulai putarannya sendiri. Jenis kapasitor yang digunakan (start atau run) dan nilainya disesuaikan dengan kebutuhan torsi start dan karakteristik operasi pompa air.

## Prinsip Kerja Pompa Air Motor Satu Fasa

Motor satu fasa pada pompa air berfungsi sebagai penggerak utama yang menyediakan energi mekanik berupa putaran poros. Putaran poros motor ini kemudian ditransfer ke impeler pompa, yang merupakan bagian yang berputar di dalam rumah pompa dan secara langsung berinteraksi dengan air.

Berikut adalah langkah-langkah terperinci mengenai prinsip kerja pompa air motor satu fasa:

1.  **Motor Satu Fasa Diberi Daya dan Mulai Berputar:**
    * Ketika pompa air dihidupkan, sumber tegangan AC satu fasa dialirkan ke motor.
    * Seperti yang telah dijelaskan sebelumnya, motor satu fasa memerlukan mekanisme bantu start (seperti kapasitor) untuk menciptakan medan magnet putar awal di stator.
    * Medan magnet putar ini menginduksi arus pada rotor sangkar tupai, menghasilkan torsi awal yang menyebabkan rotor mulai berputar.
    * Setelah mencapai kecepatan kerja (biasanya sekitar 70-80% dari kecepatan nominal), mekanisme start (misalnya saklar sentrifugal) melepaskan kumparan bantu (dan kapasitor start pada beberapa jenis motor), dan motor terus berputar menggunakan kumparan utama.

2.  **Transfer Energi Putar ke Impeler Pompa:**
    * Poros rotor motor secara langsung terhubung dengan poros impeler pompa. Sambungan ini bisa menggunakan kopling (coupling) atau poros motor dan poros impeler merupakan satu kesatuan (desain monoblok).
    * Putaran poros motor dengan kecepatan tinggi (biasanya ribuan putaran per menit, RPM) ditransfer sepenuhnya ke impeler.

3.  **Impeler Berputar dan Menciptakan Gaya Sentrifugal:**
    * Impeler memiliki bilah-bilah melengkung (vane). Saat impeler berputar dengan kecepatan tinggi di dalam rumah pompa (casing pompa), bilah-bilah ini mendorong air yang ada di antara bilah-bilahnya.
    * Dorongan ini menyebabkan air ikut berputar bersama impeler. Karena adanya gerakan memutar ini, air mengalami gaya sentrifugal yang kuat. Gaya sentrifugal ini mendorong air menjauhi pusat impeler ke arah luar, menuju pinggiran rumah pompa.

4.  **Proses Pengisapan (Suction):**
    * Saat air terlempar keluar dari pusat impeler menuju pinggiran karena gaya sentrifugal, ini menciptakan area bertekanan rendah (vakum parsial) di pusat impeler, tepatnya di "mata" impeler (impeller eye).
    * Tekanan atmosfer (atau tekanan permukaan air pada sumber air) yang lebih tinggi di luar pompa akan mendorong air dari sumber air (sumur, tangki, dll.) masuk ke dalam pipa hisap (suction pipe) dan terus masuk ke area bertekanan rendah di pusat impeler. Inilah yang disebut proses pengisapan. Pompa sentrifugal "mengisap" air bukan dengan menariknya, melainkan dengan mengurangi tekanan di dalamnya sehingga tekanan eksternal mendorong air masuk.

5.  **Proses Pengeluaran (Discharge) dan Peningkatan Tekanan:**
    * Air yang telah masuk ke dalam impeler terus didorong keluar oleh bilah-bilah impeler karena gaya sentrifugal. Air keluar dari impeler dengan kecepatan yang tinggi.
    * Air yang berkecepatan tinggi ini kemudian memasuki area rumah pompa yang berbentuk volute (seperti siput) atau diffuser. Bentuk rumah pompa ini didesain sedemikian rupa sehingga luas penampang alirannya membesar secara bertahap.
    * Ketika air berkecepatan tinggi memasuki area yang luas penampangnya membesar, kecepatannya menurun. Berdasarkan prinsip fisika, penurunan kecepatan fluida akan diikuti dengan peningkatan tekanan statisnya (konversi energi kinetik menjadi energi potensial tekanan, sesuai Prinsip Bernoulli).
    * Peningkatan tekanan ini membuat air memiliki energi tekanan yang cukup untuk didorong keluar melalui pipa keluar (discharge pipe) menuju tujuan yang diinginkan (misalnya, ke tangki penyimpanan, keran, atau sistem irigasi).

6.  **Operasi Berkelanjutan:**
    * Selama motor tetap berputar dan ada suplai air yang cukup di sisi hisap, proses pengisapan dan pengeluaran ini berlangsung secara kontinu, menciptakan aliran air dari sumber ke tujuan dengan tekanan tertentu.

**Singkatnya:** Motor satu fasa mengubah energi listrik menjadi energi putar. Putaran ini menggerakkan impeler pompa. Impeler menggunakan gaya sentrifugal untuk menciptakan area bertekanan rendah di pusatnya, menyebabkan air terisap masuk. Air yang terisap kemudian dilempar keluar oleh impeler, dan bentuk rumah pompa mengubah energi kecepatan air menjadi energi tekanan, memungkinkan air didorong ke tempat yang lebih tinggi atau jarak yang lebih jauh. Seluruh proses ini dimulai dan dipertahankan oleh kerja motor satu fasa.

## Gulung Ulang Motor Pompa Air

Rewinding, atau menggulung ulang motor satu fasa pompa air, dilakukan ketika kumparan di dalam stator motor mengalami kerusakan, seperti putus, terbakar, atau terjadi hubung singkat, yang menyebabkan motor tidak dapat beroperasi dengan baik atau bahkan mati total.

### Proses Menggulung Ulang
Proses rewinding ini memerlukan ketelitian dan pemahaman yang baik tentang konstruksi dan data teknis motor. Berikut adalah langkah-langkah umum dalam melakukan rewinding motor satu fasa pompa air:

#### Tahap 1: Persiapan dan Pembongkaran

1.  **Identifikasi Masalah:** Pastikan bahwa masalah pada motor memang disebabkan oleh kerusakan kumparan, bukan komponen lain seperti kapasitor, saklar sentrifugal, atau masalah mekanis pada pompa. Pengujian awal seperti pengukuran resistansi kumparan dan pengujian isolasi (menggunakan Megger) dapat membantu mendiagnosis kerusakan kumparan.
2.  **Dokumentasi Awal:** Sebelum membongkar, amati dan catat semua detail eksternal motor, termasuk merk, model, spesifikasi pada plat nama (tegangan, daya, arus, kecepatan, frekuensi), dan jenis motor (misalnya, kapasitor start, kapasitor run). Ambil foto dari berbagai sudut jika perlu.
3.  **Penandaan:** Beri tanda pada bagian rumah motor (body) dan tutup motor (end shield) sebelum membongkar. Ini sangat penting untuk memastikan bahwa saat perakitan kembali, posisi relatif antara stator dan rumah motor serta posisi tutup motor tepat seperti semula, yang mempengaruhi keselarasan bantalan dan celah udara.
4.  **Pembongkaran Motor:**
    * Lepaskan motor dari pompa jika merupakan unit terpisah, atau bongkar bagian pompa yang terhubung dengan motor jika desainnya monoblok.
    * Lepaskan baut atau pengunci yang menahan tutup motor pada rumah motor.
    * Secara hati-hati pisahkan tutup motor dari rumah motor. Mungkin diperlukan sedikit ketukan ringan dengan palu karet atau kayu, atau menggunakan *puller* jika ada bagian yang macet. Jangan merusak poros atau bagian lain.
    * Tarik keluar rotor dari stator. Catat posisi rotor dan *keyway* (alur pasak) relatif terhadap alur stator jika ada tanda.
    * Lepaskan saklar sentrifugal dan mekanismenya dari poros rotor dan tutup motor jika ada. Perhatikan cara kerjanya dan posisinya.
    * Lepaskan kapasitor dari dudukannya dan catat sambungan kabelnya.
    * Lepaskan kotak terminal dan catat semua sambungan kabel dari kumparan motor ke terminal dan komponen eksternal lainnya. Gambarlah diagram pengawatan asli jika memungkinkan.

#### Tahap 2: Analisis dan Pelepasan Kumparan Lama

1.  **Analisis Kumparan Lama:** Setelah stator terpisah, perhatikan dengan saksama kumparan lama di dalam alur stator.
    * **Identifikasi Kumparan Utama dan Bantu:** Bedakan antara kumparan utama (biasanya kawat lebih besar) dan kumparan bantu (kawat lebih kecil). Catat posisi relatif keduanya (berjarak 90 derajat listrik).
    * **Perhatikan Pola Gulungan:** Amati pola gulungan kumparan (misalnya, konsentris atau lap winding), jumlah kelompok kumparan, dan langkah kumparan (coil pitch - jumlah alur yang dilewati satu sisi kumparan ke sisi lainnya). Gambarlah bentangan (winding diagram) kasar dari pola lilitan yang ada. Ini sangat krusial untuk mereproduksi lilitan baru.
    * **Hitung Jumlah Lilitan:** Ini adalah langkah yang paling memakan waktu dan memerlukan ketelitian. Pilih satu atau beberapa kumparan dari setiap kelompok kumparan (utama dan bantu) secara acak dan hitung jumlah lilitannya dengan hati-hati saat kawat dilepas. Lakukan ini untuk beberapa kumparan dalam satu kelompok dan rata-ratakan hasilnya untuk mendapatkan perkiraan jumlah lilitan per kumparan.
    * **Ukur Diameter Kawat:** Ukur diameter kawat tembaga berinsulasi email dari kumparan utama dan kumparan bantu menggunakan mikrometer atau alat ukur yang akurat. Diameter kawat ini sangat penting untuk menentukan ukuran kawat pengganti. Catat juga jenis insulasi email kawat.
    * **Perhatikan Isolasi Alur:** Perhatikan jenis dan kondisi bahan isolasi (biasanya prespan atau mika) yang digunakan untuk melapisi alur stator sebelum kumparan dimasukkan.

2.  **Pelepasan Kumparan Lama:**
    * Potong salah satu sisi kumparan lama yang menonjol di luar alur stator menggunakan tang potong atau pahat kecil.
    * Panaskan stator secara perlahan menggunakan *hot air gun* atau oven pada suhu rendah. Pemanasan ini membantu melunakkan pernis atau lak yang mengikat kumparan, sehingga lebih mudah dilepas.
    * Gunakan pahat, obeng kuat, dan palu untuk mencongkel dan menarik keluar sisa-sisa kumparan dan isolasi dari alur stator. Lakukan dengan hati-hati agar tidak merusak inti besi laminasi stator.
    * Bersihkan semua alur stator dari sisa kawat, isolasi, dan kotoran lainnya.

#### Tahap 3: Perhitungan Data Lilitan dan Persiapan Stator

1.  **Verifikasi dan Perhitungan Data Lilitan Baru:**
    * Berdasarkan data jumlah lilitan per kumparan, diameter kawat, pola gulungan, dan langkah kumparan yang dicatat dari kumparan lama, hitung data lilitan baru. Data ini harus sama atau sangat mirip dengan aslinya untuk mendapatkan karakteristik motor yang serupa. Jika motor asli sudah pernah direwinding dan performanya buruk, mungkin diperlukan penyesuaian data lilitan oleh ahli.
    * Tentukan total berat kawat tembaga yang dibutuhkan untuk kumparan utama dan bantu berdasarkan jumlah lilitan, diameter kawat, dan perkiraan panjang rata-rata lilitan.

2.  **Persiapan Bahan Isolasi:**
    * Potong bahan isolasi alur (prespan atau mika) sesuai dengan ukuran alur stator. Bentuk isolasi alur biasanya persegi panjang yang dilipat atau dibentuk U untuk melapisi dinding dan dasar alur.
    * Siapkan bahan isolasi antar-kelompok kumparan dan isolasi penutup alur (biasanya semacam bilah bambu atau bahan isolasi keras lainnya) yang akan dimasukkan setelah kumparan selesai dimasukkan ke alur.

3.  **Pelapisan Alur Stator:**
    * Masukkan lembaran isolasi alur yang sudah dipotong ke dalam setiap alur stator dengan rapi. Pastikan isolasi menutupi seluruh permukaan alur untuk mencegah kawat berinsulasi bersentuhan langsung dengan inti besi stator.

#### Tahap 4: Penggulungan dan Pemasukan Kumparan Baru

1.  **Pembuatan Mal Kumparan (Coil Form):** Buat mal (cetakan) sesuai dengan ukuran dan bentuk kumparan asli. Mal ini biasanya dapat disetel ukurannya sesuai dengan langkah kumparan yang berbeda dalam satu kelompok.
2.  **Penggulungan Kumparan:** Gulung kawat tembaga berinsulasi email yang baru (sesuai dengan diameter kawat yang diukur) pada mal sesuai dengan jumlah lilitan yang telah dihitung untuk setiap kumparan. Gulung secara terpisah untuk kumparan utama dan kumparan bantu. Usahakan hasil gulungan rapi agar mudah dimasukkan ke alur.
3.  **Pemasukan Kumparan ke Alur:** Ini adalah tahap yang paling sulit dan memerlukan kesabaran.
    * Mulai dengan kumparan utama. Masukkan sisi-sisi kumparan utama ke dalam alur-alur yang sesuai dengan pola dan langkah kumparan yang telah ditentukan. Gunakan alat bantu seperti bilah plastik atau kayu untuk mendorong kawat masuk ke dalam alur.
    * Setelah satu sisi kumparan dimasukkan, masukkan isolasi penutup alur untuk mengamankan kawat di dalamnya.
    * Ulangi proses ini untuk sisi kumparan yang lain pada alur pasangannya sesuai langkah kumparan.
    * Lanjutkan memasukkan seluruh kumparan utama sesuai dengan pola gulungan.
    * Setelah kumparan utama selesai dimasukkan, masukkan kumparan bantu ke dalam alur-alur yang sesuai dengan posisinya (berjarak 90 derajat listrik dari kumparan utama) dan pola gulungan serta langkah kumparannya. Hati-hati agar tidak merusak insulasi kawat kumparan utama yang sudah terpasang.

#### Tahap 5: Pengawatan dan Pengujian Isolasi**

1.  **Penyambungan Kumparan:** Sambung ujung-ujung kumparan di luar alur sesuai dengan diagram pengawatan motor satu fasa (seri atau paralel dalam setiap kelompok, dan hubungan antara kumparan utama dan bantu). Gunakan metode penyambungan yang baik (misalnya, disolder atau dikrim) dan lapisi sambungan dengan isolasi tahan panas (misalnya, *heat shrink tube* atau selongsong insulasi). Pastikan polaritas setiap kelompok kumparan benar agar menghasilkan kutub magnet yang tepat.
2.  **Penyambungan ke Kabel Terminal:** Sambungkan ujung-ujung kumparan utama dan bantu yang sudah terhubung ke kabel yang akan dihubungkan ke terminal motor. Pastikan identifikasi kabel (misalnya, kabel utama, kabel bantu, kabel common) jelas.
3.  **Pengikatan Kumparan:** Rapikan dan ikat kumparan yang menonjol di kedua ujung stator menggunakan tali khusus yang kuat (misalnya, benang nilon atau dacron yang dipernis). Pengikatan ini penting agar kumparan kokoh, tidak bergeser akibat getaran, dan tidak menyentuh rotor.
4.  **Pengujian Isolasi Awal:** Lakukan pengujian isolasi antara kumparan dengan bodi stator (ground) menggunakan Megger untuk memastikan tidak ada kawat yang terkelupas dan menyentuh inti besi. Juga ukur resistansi masing-masing kumparan (utama dan bantu) menggunakan multimeter untuk memverifikasi kontinuitas dan kesesuaian nilainya dengan perhitungan.

#### Tahap 6: Impregnasi (Varnishing) dan Pengeringan

1.  **Impregnasi:** Celupkan stator yang sudah tergulung ke dalam cairan pernis isolasi listrik (varnish) atau oleskan pernis secara merata ke seluruh permukaan kumparan. Proses ini disebut impregnasi. Tujuan impregnasi adalah untuk:
    * Mengisi celah-celah kecil di antara lilitan, meningkatkan kekuatan mekanik kumparan dan mencegah pergerakan lilitan.
    * Meningkatkan kekuatan dielektrik insulasi, mencegah terjadinya hubung singkat antar lilitan.
    * Melindungi kumparan dari kelembaban, debu, dan bahan kimia korosif.
    * Membantu perpindahan panas dari kumparan ke inti stator dan rumah motor.
2.  **Pengeringan:** Setelah diimpregnasi, keringkan stator di dalam oven dengan suhu dan waktu yang sesuai dengan spesifikasi pernis yang digunakan. Proses pengeringan yang tepat akan memastikan pernis mengeras dengan baik.

#### Tahap 7: Perakitan Kembali dan Pengujian Akhir

1.  **Pembersihan Komponen:** Bersihkan semua komponen motor yang lain (rumah motor, tutup motor, rotor, bantalan, saklar sentrifugal) dari kotoran, karat, atau sisa-sisa lama.
2.  **Pemasangan Bantalan Baru (jika perlu):** Jika bantalan lama sudah aus atau menimbulkan suara bising, ganti dengan bantalan baru yang sesuai. Lumasi bantalan baru jika diperlukan.
3.  **Perakitan Motor:** Pasang kembali semua komponen motor secara berurutan, dimulai dari pemasangan bantalan pada tutup motor dan/atau rumah motor, pemasangan rotor ke dalam stator (perhatikan tanda penandaan posisi relatif), pemasangan saklar sentrifugal pada poros dan tutup, penyambungan kabel kumparan ke terminal, pemasangan kembali tutup motor ke rumah motor (perhatikan tanda penandaan dan kencangkan baut secara merata), dan pemasangan kembali komponen eksternal lainnya seperti kipas dan penutup kipas.
4.  **Pengujian Akhir:** Setelah motor selesai dirakit, lakukan serangkaian pengujian:
    * **Pengujian Tahanan Isolasi:** Ukur kembali tahanan isolasi motor secara keseluruhan menggunakan Megger. Nilainya harus tinggi (biasanya dalam MegaOhm).
    * **Pengukuran Resistansi Kumparan:** Ukur kembali resistansi kumparan utama dan bantu di terminal motor.
    * **Pengujian Tanpa Beban:** Hubungkan motor ke sumber tegangan satu fasa yang sesuai tanpa terhubung ke pompa. Motor seharusnya berputar dengan lancar dan tanpa suara atau getaran abnormal. Ukur arus tanpa beban dan kecepatan putar. Periksa apakah motor dapat start sendiri dengan baik (jika jenisnya self-starting).
    * **Pengujian Berbeban (dengan Pompa):** Hubungkan kembali motor dengan pompa dan sumber air. Hidupkan motor dan amati kinerjanya. Periksa apakah pompa dapat mengisap dan mengeluarkan air dengan baik sesuai spesifikasi. Ukur arus saat berbeban penuh dan pastikan tidak melebihi nilai nominal. Amati suhu motor selama operasi normal.

Rewinding motor satu fasa pompa air adalah proses perbaikan yang kompleks. Keberhasilan rewinding sangat bergantung pada ketelitian dalam mencatat data lilitan asli, kualitas bahan yang digunakan (kawat tembaga, isolasi, pernis), dan ketepatan dalam proses pengerjaan dan pengawatan. Rewinding yang dilakukan dengan benar dapat mengembalikan fungsi motor dan memperpanjang masa pakainya.

### Formulasi

Desain motor listrik melibatkan prinsip-prinsip elektromagnetisme, rangkaian listrik AC, dan mekanika. Tujuan utamanya adalah mengubah energi listrik menjadi energi mekanik seefisien mungkin sambil memenuhi persyaratan kinerja (daya, torsi start, kecepatan).

**1. Jumlah Alur Stator (Stator Slots)**

Jumlah alur pada stator ($Q_s$) bukanlah nilai tunggal yang kaku untuk semua motor, tetapi dipilih berdasarkan beberapa faktor yang terkait dengan jumlah kutub ($P$), jenis belitan (konsentris atau jerat/lap), dan keinginan untuk mendistribusikan kumparan secara merata untuk menghasilkan distribusi medan magnet yang mendekati sinusoidal.

* **Hubungan dengan Jumlah Kutub:** Motor pompa air umumnya adalah motor 2-kutub atau 4-kutub. Jumlah alur biasanya dipilih sebagai kelipatan genap dari jumlah kutub, atau setidaknya memungkinkan penempatan kumparan utama dan bantu yang terpisah 90 derajat listrik.
* **Alur per Kutub per Fasa:** Konsep penting dalam desain belitan adalah jumlah alur per kutub per fasa ($q$). Meskipun motor satu fasa hanya memiliki satu sumber fasa, pada dasarnya ia memiliki dua belitan (utama dan bantu) yang diperlakukan seperti dua fasa yang terpisah 90 derajat listrik saat start. Jadi, dalam konteks desain belitan, kita bisa mempertimbangkan seolah-olah ada "dua fasa" yang didistribusikan. Jumlah alur per kutub per fasa dihitung sebagai:
    $q = \frac{Q_s}{2 \times P \times \text{jumlah "fasa"}}$
    Untuk motor satu fasa, jumlah "fasa" ini biasanya 2 (kumparan utama dan bantu). Nilai $q$ biasanya adalah bilangan bulat atau pecahan sederhana. Desainer berusaha memiliki $q \geq 1$ untuk mendapatkan keuntungan dari belitan terdistribusi (distribusi medan magnet yang lebih baik).
* **Contoh Umum:** Untuk motor 4-kutub ($P=4$), jumlah alur yang umum dipilih adalah 24, 32, atau 36.
    * Jika $Q_s = 24$, $P=4$, jumlah "fasa" = 2, maka $q = 24 / (2 \times 4 \times 2) = 24 / 16 = 1.5$. Ini berarti rata-rata ada 1.5 alur per kutub per belitan.
    * Jika $Q_s = 36$, $P=4$, jumlah "fasa" = 2, maka $q = 36 / (2 \times 4 \times 2) = 36 / 16 = 2.25$.
* **Fisika di Baliknya:** Mendistribusikan kumparan dalam beberapa alur per kutub (memiliki $q > 0$) membantu menghasilkan distribusi gaya gerak magnet (MMF) di celah udara yang lebih mendekati bentuk gelombang sinusoidal. Medan magnet sinusoidal menghasilkan torsi yang lebih halus dan mengurangi harmonisa yang dapat menyebabkan getaran dan kerugian tambahan. Penempatan kumparan utama dan bantu dengan pergeseran 90 derajat listrik di antara keduanya adalah kunci untuk menciptakan medan magnet putar (meskipun elips pada motor satu fasa) untuk start.

**2. Penentuan Ukuran Diameter Kawat Email (Koil Kumparan)**

Ukuran diameter kawat email (atau lebih tepatnya luas penampang kawat) ditentukan berdasarkan arus yang akan mengalir melaluinya dan kerapatan arus (current density) yang diizinkan pada bahan kawat (tembaga).

* **Penentuan Arus Nominal:** Arus yang mengalir pada kumparan utama (dan kumparan bantu saat start) berhubungan langsung dengan daya output motor ($P_{out}$), tegangan suplai ($V$), efisiensi ($\eta$), dan faktor daya ($cos\phi$) motor. Arus nominal motor ($I_{nominal}$) dapat diperkirakan menggunakan rumus daya input pada rangkaian AC satu fasa:
    $P_{in} = V \times I_{nominal} \times cos\phi$
    Karena $P_{out} = \eta \times P_{in}$, maka:
    $I_{nominal} = \frac{P_{out}}{\eta \times V \times cos\phi}$
    Nilai $\eta$ dan $cos\phi$ biasanya merupakan perkiraan atau berdasarkan data motor sejenis. Arus pada kumparan utama selama operasi normal akan mendekati $I_{nominal}$. Arus pada kumparan bantu saat start bisa jauh lebih tinggi.
* **Penentuan Kerapatan Arus:** Kerapatan arus ($J$) adalah besarnya arus per satuan luas penampang kawat (misalnya, Ampere per mm²). Nilai $J$ yang diizinkan tergantung pada bahan kawat (tembaga lebih tinggi dari aluminium), jenis insulasi, dan sistem pendinginan motor. Kerapatan arus yang lebih tinggi berarti kawat lebih kecil, tetapi motor akan lebih panas karena kerugian $I^2R$ yang lebih besar. Nilai $J$ untuk motor berpendingin udara alami umumnya berkisar antara 3 hingga 6 A/mm². Desainer memilih nilai $J$ berdasarkan keseimbangan antara ukuran motor, biaya (jumlah tembaga), dan kenaikan suhu yang diizinkan.
* **Perhitungan Luas Penampang Kawat:** Luas penampang kawat ($A_{wire}$) dihitung dengan membagi arus yang diharapkan dengan kerapatan arus yang diizinkan:
    $A_{wire} = \frac{I}{J}$
    Untuk kumparan utama, $I$ adalah arus nominal motor. Untuk kumparan bantu, perhitungan lebih kompleks karena arusnya hanya saat start, tetapi puncaknya bisa tinggi. Namun, kumparan bantu didesain untuk waktu operasi yang singkat. Seringkali, ukuran kawat bantu dipilih agar memiliki resistansi total yang cukup untuk pergeseran fasa yang diinginkan bersama kapasitor.
* **Penentuan Diameter Kawat:** Setelah mendapatkan luas penampang kawat ($A_{wire}$), diameter kawat telanjang ($d_{wire}$) dapat dihitung menggunakan rumus luas lingkaran:
    $A_{wire} = \frac{\pi \times d_{wire}^2}{4}$
    $d_{wire} = \sqrt{\frac{4 \times A_{wire}}{\pi}}$
    Diameter ini adalah diameter kawat tembaga *tanpa* insulasi email. Kawat email yang sebenarnya akan sedikit lebih besar karena lapisan insulasi. Standar kawat email (seperti AWG, SWG, atau standar metrik) menyediakan tabel yang menghubungkan diameter kawat telanjang dengan luas penampang dan diameter total dengan insulasi.
* **Hubungan dengan Dimensi Stator:** Diameter stator (bore diameter) dan tebal stator (core length) *tidak secara langsung* menentukan diameter kawat. Namun, dimensi ini menentukan **luas alur** ($A_{slot}$). Total luas yang dibutuhkan oleh semua lilitan kumparan (jumlah total lilitan $\times$ luas penampang kawat) harus muat di dalam total luas alur stator yang tersedia, dengan mempertimbangkan faktor pengisian alur (slot fill factor - rasio luas tembaga terhadap total luas alur, biasanya antara 0.3 hingga 0.5 untuk motor kecil). Jika kawat yang dibutuhkan (berdasarkan arus dan $J$) terlalu besar sehingga tidak muat di alur, maka desainer harus berkompromi (misalnya, meningkatkan ukuran stator, menerima kenaikan suhu yang lebih tinggi dengan $J$ lebih tinggi, atau mengurangi jumlah lilitan yang akan mempengaruhi tegangan).

**3. Penentuan Jumlah Lilitan Kumparan Utama dan Kumparan Bantu**

Jumlah lilitan pada kumparan utama dan bantu ditentukan berdasarkan tegangan kerja motor dan fluks magnetik di celah udara.

* **Jumlah Lilitan Kumparan Utama ($N_{main}$):** Jumlah lilitan kumparan utama ditentukan sebagian besar oleh Persamaan GGL (Gaya Gerak Listrik) induksi pada mesin AC. GGL yang terinduksi pada kumparan utama selama operasi berjalan hampir sama dengan tegangan suplai ($V$) dikurangi sedikit rugi tegangan. Persamaan GGL (bentuk RMS) adalah:
    $E_{main} \approx 4.44 \times k_{w\_main} \times f \times N_{main} \times \Phi_p$
    Di mana:
    * $E_{main}$ adalah GGL terinduksi pada kumparan utama (sekitar $V$).
    * $k_{w\_main}$ adalah faktor belitan (winding factor) kumparan utama, yang nilainya sedikit kurang dari 1 dan bergantung pada distribusi kumparan di alur (langkah kumparan dan distribusi per kutub).
    * $f$ adalah frekuensi suplai (misalnya, 50 Hz atau 60 Hz).
    * $N_{main}$ adalah jumlah total lilitan kumparan utama.
    * $\Phi_p$ adalah fluks magnetik maksimum per kutub di celah udara (dalam Weber).

    Fluks per kutub ($\Phi_p$) berhubungan dengan kerapatan fluks magnetik ($B$) di celah udara dan luas area per kutub ($A_p$). Luas area per kutub bergantung pada dimensi stator (diameter bore $D$ dan panjang inti $L$):
    $\Phi_p \approx B \times A_p = B \times \frac{\pi \times D \times L}{\text{jumlah kutub } P}$
    Kerapatan fluks $B$ adalah parameter desain penting yang memengaruhi saturasi inti besi dan kerugian besi. Nilai $B$ dipilih berdasarkan karakteristik bahan inti laminasi, biasanya dalam rentang 1.0 hingga 1.5 Tesla.

    Dengan menggabungkan rumus GGL dan fluks, jumlah lilitan kumparan utama dapat diperkirakan:
    $N_{main} \approx \frac{V}{4.44 \times k_{w\_main} \times f \times B \times \frac{\pi \times D \times L}{P}}$
    Jadi, diameter bore stator ($D$) dan panjang inti stator ($L$) memang memengaruhi jumlah lilitan yang dibutuhkan melalui parameter fluks per kutub.

* **Jumlah Lilitan Kumparan Bantu ($N_{aux}$):** Penentuan jumlah lilitan kumparan bantu lebih kompleks karena tujuannya adalah untuk menciptakan pergeseran fasa yang optimal dengan kumparan utama saat start. Jumlah lilitan bantu ($N_{aux}$) dan ukuran kawatnya, bersama dengan nilai kapasitor start (jika ada), menentukan impedansi rangkaian bantu dan, oleh karena itu, fasa arus bantu relatif terhadap arus utama.
    * Rasio jumlah lilitan kumparan bantu terhadap kumparan utama ($N_{aux}/N_{main}$) merupakan parameter desain yang kritis untuk torsi start.
    * Seringkali, kumparan bantu memiliki jumlah lilitan yang sedikit lebih banyak atau lebih sedikit dari kumparan utama, tetapi dengan diameter kawat yang lebih kecil (resistansi lebih tinggi).
    * Desain kumparan bantu dan pemilihan kapasitor start (pada motor kapasitor) seringkali dilakukan dengan perhitungan iteratif atau menggunakan perangkat lunak desain motor untuk mengoptimalkan torsi start sambil membatasi arus start.
    * Tidak ada rumus sederhana yang hanya berdasarkan dimensi stator untuk menentukan $N_{aux}/N_{main}$; ini sangat bergantung pada kinerja start yang diinginkan dan karakteristik kumparan utama serta komponen eksternal (kapasitor). Sebuah titik awal kasar mungkin didasarkan pada mempertahankan kerapatan fluks yang seimbang antara kumparan utama dan bantu saat start.

**Kesimpulan:**

Jumlah alur stator pada motor satu fasa pompa air dipilih berdasarkan jumlah kutub dan kebutuhan distribusi belitan untuk mendapatkan medan magnet yang baik. Ukuran diameter kawat email ditentukan oleh arus yang diharapkan (berhubungan dengan daya motor dan tegangan) dan kerapatan arus yang diizinkan, dengan batasan fisik berupa luas alur stator yang tersedia. Jumlah lilitan kumparan utama ditentukan oleh tegangan kerja motor, frekuensi, faktor belitan, dan fluks magnetik per kutub (yang dipengaruhi oleh diameter bore dan panjang inti stator). Jumlah lilitan kumparan bantu dan rasionya terhadap kumparan utama, bersama dengan komponen bantu start (kapasitor), ditentukan berdasarkan persyaratan torsi start dan merupakan hasil dari desain yang lebih kompleks yang menyeimbangkan parameter listrik dan magnetik. Meskipun dimensi stator (diameter dan tebal) tidak secara langsung memberikan rumus sederhana untuk *semua* parameter lilitan, dimensi tersebut memainkan peran penting dalam menentukan luas untuk fluks magnetik dan ruang yang tersedia untuk menempatkan kumparan dengan jumlah lilitan dan ukuran kawat yang diperlukan.

Tentu, mari kita telaah kembali secara terperinci aspek fisika dan matematika yang mendasari desain stator motor satu fasa, khususnya untuk aplikasi pompa air, termasuk penentuan jumlah alur stator, ukuran kawat email, dan jumlah lilitan kumparan utama dan bantu.

Desain motor listrik adalah aplikasi langsung dari prinsip-prinsip elektromagnetisme dan teori rangkaian listrik. Tujuannya adalah mengoptimalkan konversi energi listrik menjadi energi mekanik melalui interaksi medan magnet yang dihasilkan oleh stator dan rotor.

**1. Jumlah Alur Stator ($Q_s$)**

Alur atau slot pada stator adalah rongga memanjang yang berfungsi sebagai tempat untuk menempatkan kumparan kawat (lilitan). Jumlah alur stator ($Q_s$) bukanlah angka sembarang, melainkan dipilih berdasarkan beberapa kriteria desain untuk mencapai kinerja motor yang optimal, terutama terkait dengan pembentukan medan magnet.

* **Tujuan Fisik:** Fungsi utama alur adalah menahan dan menata kumparan stator. Penempatan kumparan dalam alur-alur yang terdistribusi di sekeliling stator memungkinkan pembentukan distribusi medan gaya gerak magnet (GGM) atau *Magnetomotive Force* (MMF) di celah udara yang mendekati bentuk gelombang sinusoidal. Distribusi MMF yang sinusoidal ini penting karena menghasilkan medan magnet yang lebih "bersih" (sedikit harmonisa) yang berinteraksi dengan rotor untuk menghasilkan torsi putar yang halus dan efisien.
* **Hubungan dengan Jumlah Kutub ($P$):** Motor pompa air umumnya didesain sebagai motor 2-kutub ($P=2$) atau 4-kutub ($P=4$). Jumlah alur ($Q_s$) biasanya merupakan kelipatan genap dari jumlah kutub. Pemilihan $Q_s$ harus memungkinkan penempatan kumparan utama dan kumparan bantu yang terpisah secara spasial sebesar 90 derajat listrik. Jarak 90 derajat listrik ini setara dengan $\frac{180 \text{ derajat listrik}}{\text{jumlah kutub } P} \times \frac{90 \text{ derajat listrik}}{180 \text{ derajat listrik}} = \frac{180}{P} \times \frac{1}{2} = \frac{90}{P}$ derajat mekanik, yang setara dengan sejumlah alur mekanik.
* **Alur per Kutub per Fasa ($q$):** Untuk mendistribusikan kumparan secara merata, desainer menggunakan konsep alur per kutub per fasa ($q$). Meskipun motor satu fasa hanya memiliki satu fasa listrik, desain belitan statornya terdiri dari kumparan utama dan kumparan bantu yang secara fisik terpisah dan diberi pergeseran fasa listrik (menggunakan kapasitor atau cara lain) saat start. Dalam konteks desain belitan untuk mendapatkan medan putar, seringkali ini diperlakukan seperti motor dengan "dua fasa" (kumparan utama dan bantu). Rumusnya:
    $q = \frac{Q_s}{2 \times P \times \text{jumlah "fasa"}}$
    Pada motor satu fasa, jumlah "fasa" ini adalah 2. Nilai $q$ biasanya dipilih sebagai bilangan bulat positif atau pecahan sederhana untuk memudahkan pembuatan dan penempatan kumparan. Misalnya, $q=1, 1.5, 2, 2.5$, dst.
* **Contoh Jumlah Alur:** Untuk motor 4-kutub ($P=4$), jumlah alur yang umum adalah 24 atau 36.
    * Jika $Q_s = 24$ alur, maka $q = \frac{24}{2 \times 4 \times 2} = \frac{24}{16} = 1.5$. Artinya, rata-rata ada 1.5 alur per kutub untuk kumparan utama dan 1.5 alur per kutub untuk kumparan bantu.
    * Jika $Q_s = 36$ alur, maka $q = \frac{36}{2 \times 4 \times 2} = \frac{36}{16} = 2.25$.
* **Fisika Pemilihan Alur:** Semakin banyak alur per kutub per fasa ($q$ yang lebih besar), semakin baik distribusi kumparan dan semakin mendekati sinusoidal bentuk gelombang MMF yang dihasilkan. Ini mengurangi harmonisa MMF yang tidak diinginkan dan meningkatkan efisiensi serta mengurangi kebisingan dan getaran motor. Namun, jumlah alur yang terlalu banyak juga meningkatkan biaya produksi dan kompleksitas pembuatan. Oleh karena itu, pemilihan $Q_s$ adalah kompromi desain. Untuk motor pompa air kecil, $Q_s=24$ atau 36 untuk motor 4-kutub adalah pilihan yang umum.

**2. Penentuan Ukuran Diameter Kawat Email (Koil Kumparan)**

Ukuran kawat email (diameter atau luas penampangnya) untuk kumparan utama dan kumparan bantu ditentukan berdasarkan arus listrik yang akan mengalir melaluinya dan kemampuan kawat tersebut membuang panas tanpa melebihi batas suhu insulasi.

* **Prinsip Dasar:** Kumparan motor berfungsi mengalirkan arus listrik untuk menghasilkan medan magnet. Saat arus mengalir, terjadi kerugian daya akibat resistansi kawat ($P_{rugi} = I^2 \times R$). Kerugian ini berubah menjadi panas. Kawat harus memiliki luas penampang yang cukup besar agar panas yang dihasilkan dapat dibuang ke lingkungan tanpa merusak insulasi kawat.
* **Penentuan Arus Listrik:** Arus listrik yang mengalir pada kumparan utama selama operasi normal berkaitan dengan daya output motor ($P_{out}$), tegangan suplai ($V$), efisiensi ($\eta$), dan faktor daya ($cos\phi$). Daya input listrik ($P_{in}$) pada motor AC satu fasa adalah:
    $P_{in} = V \times I_{masuk} \times cos\phi$
    Di mana:
    * $P_{in}$ adalah daya input listrik (Watt).
    * $V$ adalah tegangan suplai RMS (Volt).
    * $I_{masuk}$ adalah total arus yang ditarik motor dari suplai (Ampere).
    * $cos\phi$ adalah faktor daya motor (tidak memiliki satuan, nilainya antara 0 dan 1).

    Daya output mekanik ($P_{out}$) berkaitan dengan daya input melalui efisiensi ($\eta$):
    $P_{out} = \eta \times P_{in} = \eta \times V \times I_{masuk} \times cos\phi$
    Maka, total arus masuk dari suplai adalah:
    $I_{masuk} = \frac{P_{out}}{\eta \times V \times cos\phi}$

    Arus yang mengalir di kumparan utama ($I_{main}$) selama operasi normal adalah komponen utama dari $I_{masuk}$. Arus pada kumparan bantu ($I_{aux}$) sangat kecil saat operasi normal (pada motor CSIR) atau memiliki fasa yang berbeda (pada motor PSC/CSCR). Untuk kumparan utama, ukuran kawat ditentukan berdasarkan $I_{main}$.

* **Kerapatan Arus ($J$):** Kerapatan arus adalah besarnya arus listrik yang mengalir melalui setiap satuan luas penampang kawat. Dinyatakan dalam Ampere per milimeter persegi (A/mm²) atau Ampere per inci persegi. Kerapatan arus yang diizinkan pada kawat tembaga berinsulasi email tergantung pada seberapa baik panas dapat dikeluarkan dari kumparan. Nilai $J$ yang umum untuk motor berpendingin udara (seperti motor pompa air) berkisar antara $3 \text{ A/mm}^2$ hingga $6 \text{ A/mm}^2$. Nilai yang lebih rendah memberikan motor yang lebih dingin (efisiensi lebih baik) tetapi memerlukan lebih banyak tembaga (kawat lebih besar).
    $J = \frac{\text{Arus (I)}}{\text{Luas Penampang Kawat (A}_{wire})}$

* **Penentuan Luas Penampang Kawat:** Dari persamaan kerapatan arus, luas penampang kawat yang dibutuhkan adalah:
    $A_{wire} = \frac{I}{J}$
    Untuk kumparan utama, $I$ adalah $I_{main}$. Untuk kumparan bantu, perhitungannya berbeda; kawatnya lebih kecil karena arus start yang tinggi hanya berlangsung sesaat, tetapi resistansinya perlu dipertimbangkan untuk pergeseran fasa. Seringkali, ukuran kawat bantu dipilih berdasarkan ruang yang tersedia di alur dan pertimbangan resistansi/impedansi.

* **Penentuan Diameter Kawat:** Setelah mengetahui luas penampang kawat yang dibutuhkan ($A_{wire}$), diameter kawat tembaga telanjang ($d_{wire}$) dapat dihitung dengan rumus luas lingkaran:
    $A_{wire} = \frac{\pi \times d_{wire}^2}{4}$
    Maka, diameter kawat telanjang adalah:
    $d_{wire} = \sqrt{\frac{4 \times A_{wire}}{\pi}}$
    Diameter kawat email yang sebenarnya akan sedikit lebih besar karena lapisan insulasi. Data standar kawat email (misalnya, tabel AWG atau standar metrik) memberikan hubungan antara ukuran kawat standar, diameter telanjang, luas penampang, dan diameter berinsulasi.

* **Hubungan dengan Dimensi Stator (Diameter Bore $D$ dan Panjang Inti $L$):** Dimensi fisik stator seperti diameter bore ($D$) dan panjang inti ($L$) secara *tidak langsung* memengaruhi pemilihan ukuran kawat. Dimensi ini menentukan total volume alur yang tersedia untuk menampung kumparan. Luas penampang alur ($A_{slot}$) dikalikan dengan jumlah alur ($Q_s$) memberikan total volume (atau luas di penampang melintang) yang bisa diisi tembaga. Luas total tembaga (total lilitan $\times$ luas penampang kawat) harus sesuai dengan ruang alur, dengan mempertimbangkan faktor pengisian alur (slot fill factor) yang kurang dari 1 karena adanya insulasi alur, insulasi antar-lilitan, dan ruang kosong. Jika perhitungan berdasarkan arus dan $J$ menghasilkan kawat yang terlalu besar sehingga tidak muat di alur dengan jumlah lilitan yang dibutuhkan, maka desainer harus menyesuaikan (misalnya, memilih $J$ yang lebih tinggi, mendesain ulang stator dengan alur yang lebih besar, atau mengkompromikan parameter lain).

**3. Penentuan Jumlah Putaran Kawat Email (Lilitan) Kumparan Utama dan Kumparan Bantu**

Jumlah lilitan pada setiap kumparan (utama dan bantu) sangat penting karena menentukan GGL (tegangan) yang terinduksi pada kumparan tersebut ketika ada perubahan fluks magnetik.

* **Prinsip Dasar:** Motor induksi bekerja berdasarkan prinsip induksi elektromagnetik (Hukum Faraday). Ketika medan magnet yang berputar (atau berdenyut dan berinteraksi dengan rotor yang bergerak) memotong lilitan kumparan stator, tegangan (GGL) terinduksi pada kumparan tersebut. Besarnya GGL yang terinduksi berbanding lurus dengan laju perubahan fluks magnetik yang dilingkupi oleh kumparan dan jumlah lilitan kumparan.
* **Jumlah Lilitan Kumparan Utama ($N_{main}$):** Selama operasi normal, GGL yang terinduksi pada kumparan utama ($E_{main}$) hampir sama dengan tegangan suplai terminal motor ($V$). Rumus GGL RMS (Root Mean Square) untuk kumparan yang terdistribusi dengan fluks sinusoidal di celah udara adalah:
    $E = 4.44 \times k_w \times f \times N \times \Phi_p$
    Di mana:
    * $E$ adalah GGL RMS yang terinduksi pada kumparan (Volt). Untuk kumparan utama, $E_{main} \approx V$.
    * $4.44$ adalah konstanta yang berasal dari $\sqrt{2} \times \pi$.
    * $k_w$ adalah faktor belitan (winding factor), yang memperhitungkan bagaimana kumparan didistribusikan di alur (langkah kumparan dan distribusi per kutub). Nilainya biasanya antara 0.85 hingga 0.98, tergantung desain belitan. Untuk kumparan utama, gunakan $k_{w\_main}$.
    * $f$ adalah frekuensi suplai (Hertz, Hz). Di Indonesia umumnya 50 Hz.
    * $N$ adalah jumlah total lilitan untuk kumparan yang bersangkutan. Untuk kumparan utama, $N_{main}$.
    * $\Phi_p$ adalah fluks magnetik maksimum per kutub di celah udara (Weber, Wb).

    Fluks per kutub ($\Phi_p$) bergantung pada kerapatan fluks magnetik rata-rata di celah udara ($B_{avg}$) dan luas area efektif per kutub ($A_p$). Luas area per kutub dapat diperkirakan dari dimensi stator:
    $A_p \approx \frac{\pi \times D \times L}{P}$
    Di mana:
    * $A_p$ adalah luas area efektif per kutub (meter persegi, m²).
    * $D$ adalah diameter bore stator (meter, m).
    * $L$ adalah panjang inti stator (meter, m).
    * $P$ adalah jumlah kutub.

    Kerapatan fluks $B$ adalah parameter desain yang penting. Pemilihan nilai $B$ yang terlalu tinggi dapat menyebabkan saturasi inti besi dan meningkatkan kerugian. Nilai $B$ umumnya berkisar antara 1.0 hingga 1.5 Tesla (T).

    Dengan menggabungkan rumus GGL dan fluks, jumlah total lilitan kumparan utama dapat diperkirakan:
    $N_{main} \approx \frac{V}{4.44 \times k_{w\_main} \times f \times B \times (\frac{\pi \times D \times L}{P})}$
    Rumus ini menunjukkan bahwa jumlah lilitan kumparan utama berbanding lurus dengan tegangan suplai dan jumlah kutub, serta berbanding terbalik dengan frekuensi, faktor belitan, kerapatan fluks, diameter bore, dan panjang inti stator.

* **Jumlah Lilitan Kumparan Bantu ($N_{aux}$):** Penentuan jumlah lilitan kumparan bantu sedikit berbeda. Kumparan bantu terutama berfungsi saat motor start untuk menciptakan pergeseran fasa MMF yang diperlukan bersama dengan kumparan utama. Desainnya bertujuan untuk menghasilkan torsi start yang memadai.
    * Jumlah lilitan kumparan bantu ($N_{aux}$) dan ukuran kawatnya (serta nilai kapasitor pada motor kapasitor) menentukan impedansi rangkaian bantu.
    * Rasio jumlah lilitan kumparan bantu terhadap kumparan utama ($N_{aux}/N_{main}$) adalah parameter kunci. Rasio ini, bersama dengan perbedaan resistansi dan reaktansi antara kedua kumparan, dan impedansi kapasitor (jika ada), menentukan fasa arus yang mengalir melalui kumparan bantu relatif terhadap arus kumparan utama. Tujuannya adalah menciptakan perbedaan fasa mendekati 90 derajat listrik antara arus dan/atau MMF kedua kumparan saat start.
    * Tidak ada rumus sederhana yang universal untuk $N_{aux}$ atau rasio $N_{aux}/N_{main}$ yang hanya bergantung pada dimensi fisik stator. Nilai ini sangat bergantung pada jenis motor (kapasitor start, kapasitor run, fasa belah), nilai kapasitor (jika ada), dan torsi start yang diinginkan.
    * Secara umum, kumparan bantu seringkali memiliki jumlah lilitan yang berbeda (bisa sedikit lebih banyak atau lebih sedikit) dari kumparan utama dan menggunakan kawat dengan diameter yang lebih kecil (resistansi lebih tinggi) untuk membantu menciptakan pergeseran fasa.
    * Penentuan $N_{aux}$ dan ukuran kawatnya seringkali melibatkan perhitungan impedansi rangkaian AC yang kompleks dan seringkali melalui proses iterasi atau simulasi menggunakan perangkat lunak desain motor untuk mencapai karakteristik start yang diinginkan. Data dari motor serupa yang sudah ada juga sering menjadi acuan awal dalam proses rewinding.

**Ringkasan dan Pertimbangan Praktis dalam Rewinding:**

Dalam praktik rewinding motor pompa air, seorang teknisi atau desainer motor tidak selalu mulai dari "nol" dengan hanya dimensi stator. Mereka biasanya mengukur dan menganalisis data dari kumparan asli motor yang akan direwinding. Data asli ini (jumlah lilitan per kumparan, ukuran kawat, pola gulungan) adalah hasil dari proses desain yang telah dilakukan oleh pabrikan motor.

Meskipun rumus-rumus fisika dan matematika di atas menjelaskan hubungan mendasar antar parameter, desainer motor profesional menggunakan perangkat lunak canggih yang mempertimbangkan lebih banyak faktor (seperti efek saturasi inti, kerugian harmonisa, distribusi fluks yang tidak ideal) untuk mengoptimalkan desain.

Untuk keperluan rewinding, data yang paling penting adalah:
1.  Jumlah alur stator ($Q_s$).
2.  Jumlah kutub ($P$).
3.  Pola gulungan (konsentris atau jerat), jumlah kelompok kumparan, dan langkah kumparan untuk kumparan utama dan bantu.
4.  Jumlah lilitan per kumparan untuk setiap kelompok (utama dan bantu).
5.  Diameter kawat email (telanjang atau berinsulasi) untuk kumparan utama dan bantu.
6.  Diagram pengawatan/penyambungan kumparan.

Dengan data-data ini dari motor asli, teknisi rewinding dapat mereproduksi kumparan baru yang identik atau sangat mirip dengan aslinya, sehingga motor dapat berfungsi kembali sesuai spesifikasi. Jika data asli tidak tersedia atau motor asli sudah dimodifikasi sebelumnya, pemahaman tentang prinsip fisika dan matematika di atas (terutama hubungan V-N-$\Phi$ dan I-A-J) menjadi penting untuk memperkirakan atau menyesuaikan data lilitan.

Semoga penjelasan ini memberikan pemahaman yang lebih mendalam berdasarkan ilmu fisika dan matematika mengenai desain stator motor satu fasa pompa air.