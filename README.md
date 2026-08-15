# AI Engineer

---

## l. Perkenalan

Rekayasa AI (AI Engineering) adalah proses merancang dan mengimplementasikan sistem AI menggunakan model yang telah dilatih sebelumnya serta perangkat AI yang sudah ada untuk memecahkan masalah praktis. Insinyur AI berfokus pada penerapan AI dalam skenario dunia nyata, peningkatan pengalaman pengguna, dan otomatisasi tugas, tanpa harus mengembangkan model baru dari nol. Mereka bekerja untuk memastikan sistem AI berjalan efisien, dapat ditingkatkan skalanya (scalable), dan terintegrasi secara mulus ke dalam aplikasi bisnis; hal ini membedakan peran mereka dari Peneliti AI dan Insinyur ML, yang lebih berkonsentrasi pada pembuatan model baru atau pengembangan teori AI.

#### 1. Apa itu AI Engineer?

AI engineer adalah profesional yang memiliki keahlian dalam merancang, mengembangkan, dan mengimplementasikan sistem kecerdasan buatan (AI). Peran mereka sangat penting di berbagai industri karena mereka menciptakan aplikasi yang memungkinkan mesin melakukan tugas-tugas yang biasanya memerlukan kecerdasan manusia, seperti pemecahan masalah, pembelajaran, dan pengambilan keputusan.

#### 2. Peran dan Tanggung Jawab

Insinyur AI bertanggung jawab untuk merancang, mengembangkan, dan menerapkan sistem AI yang memecahkan masalah di dunia nyata. Peran mereka mencakup pembuatan model pembelajaran mesin (**machine learning**), penerapan alur kerja pemrosesan data, serta integrasi solusi AI ke dalam perangkat lunak atau platform yang sudah ada. Mereka menangani tugas-tugas seperti pengumpulan, pembersihan, dan pelabelan data, serta pelatihan, pengujian, dan optimalisasi model guna memastikan kinerja dan akurasi yang tinggi. Insinyur AI juga berfokus pada peningkatan skala model untuk penggunaan tahap produksi, pemantauan kinerja, dan penanganan masalah teknis. Selain itu, mereka berkolaborasi dengan ilmuwan data, pengembang perangkat lunak, dan pemangku kepentingan lainnya untuk menyelaraskan proyek AI dengan tujuan bisnis, sembari memastikan bahwa solusi yang dihasilkan andal, efisien, dan memenuhi standar etika.

#### 3. Dampak terhadap Pengembangan Produk

Rekayasa AI mengubah pengembangan produk dengan mengotomatisasi tugas, meningkatkan pengambilan keputusan berbasis data, serta memungkinkan penciptaan produk yang lebih cerdas dan personal. Teknologi ini mempercepat siklus desain, mengoptimalkan proses, serta memfasilitasi pemeliharaan prediktif, pengendalian mutu, dan pengelolaan sumber daya yang efisien. Dengan mengintegrasikan AI, perusahaan dapat berinovasi lebih cepat, menekan biaya, dan meningkatkan pengalaman pengguna, sehingga memperoleh keunggulan kompetitif di pasar.

#### 4. Insinyur AI vs. Insinyur ML

Seorang Insinyur AI menggunakan model yang telah dilatih sebelumnya dan perangkat AI yang sudah ada untuk meningkatkan pengalaman pengguna. Mereka berfokus pada penerapan AI secara praktis tanpa harus membangun model dari nol. Hal ini berbeda dengan Peneliti AI dan Insinyur ML, yang lebih berfokus pada pembuatan model baru atau pengembangan teori AI.

## ll. Cara Kerja LLM

Large Language Models (LLM) adalah sistem AI canggih yang dilatih menggunakan data teks dalam jumlah sangat besar untuk memahami, menghasilkan, dan memanipulasi bahasa manusia. Sistem ini bekerja dengan mempelajari hubungan statistik antar-kata dan frasa, yang memungkinkannya memprediksi kata berikutnya dalam suatu urutan atau menghasilkan teks yang koheren berdasarkan instruksi (prompt) yang diberikan. Kemampuan ini dicapai melalui jaringan saraf dalam (deep neural networks)—terutama dengan menggunakan arsitektur transformer—yang memungkinkan sistem menangkap ketergantungan jarak jauh dalam teks dan menghasilkan keluaran yang relevan secara kontekstual.

### Inti elemen LLM

- **Token**. dalam Large Language Models (LLM),
Token adalah unit teks dasar yang diproses oleh LLM, yang dihasilkan dengan memecah teks menjadi komponen-komponen lebih kecil seperti kata, sub-kata, atau karakter. Memahami token sangatlah penting karena model memprediksi token berikutnya dalam suatu urutan, biaya API didasarkan pada jumlah token, serta model memiliki batas maksimum token untuk input dan output.

- **Context**.
Dalam ranah Large Language Models (LLM), konteks mengacu pada informasi yang diberikan kepada model bersamaan dengan **prompt**, yang digunakan model tersebut untuk menghasilkan respons yang relevan dan koheren. Konteks mencakup pertanyaan pengguna, teks pendukung, interaksi percakapan sebelumnya, atau data lain apa pun yang membantu LLM memahami keluaran yang diinginkan. Pada dasarnya, konteks merupakan pengetahuan latar belakang dan instruksi yang memandu proses penalaran serta pembuatan respons oleh LLM.

- **Sampling Parameter**.
Parameter sampling adalah pengaturan yang mengontrol aspek keacakan dan kreativitas teks yang dihasilkan oleh LLM. Parameter ini memengaruhi cara model memilih kata berikutnya dalam suatu urutan, yang berdampak pada koherensi, keragaman, dan relevansi keseluruhan dari hasil keluaran. Penyesuaian parameter ini memungkinkan pengguna untuk menyempurnakan respons LLM bagi aplikasi tertentu, guna menyeimbangkan antara hasil keluaran yang dapat diprediksi dan aman dengan hasil yang lebih imajinatif serta eksploratif.

- **Temperature**.
adalah parameter yang digunakan dalam model bahasa yang mengontrol keacakan teks yang dihasilkan. Nilai temperature yang lebih tinggi (misalnya 1,0) menghasilkan keluaran yang lebih beragam dan tidak dapat diprediksi, karena model lebih cenderung mengambil sampel kata yang kemungkinannya lebih kecil. Sebaliknya, nilai temperature yang lebih rendah (misalnya 0,2) menghasilkan keluaran yang lebih deterministik dan konservatif, sehingga lebih memilih kata-kata yang paling mungkin menurut data pelatihan model. Pada dasarnya, ini mempengaruhi distribusi probabilitas pemilihan kata berikutnya.

- **Top-K Sampling**.
adalah metode yang digunakan oleh Large Language Model (LLM) saat menghasilkan teks untuk memilih kata berikutnya. Alih-alih mempertimbangkan seluruh kosakata, metode ini mempersempit pilihan menjadi K kata dengan probabilitas tertinggi menurut prediksi model. Nilai rendah (1-10) menghasilkan keluaran yang konservatif dan faktual. Nilai sedang (20-50) menyeimbangkan kreativitas dan kualitas. Nilai tinggi (50+) memungkinkan keluaran yang beragam dan kreatif. Gunakan nilai K rendah untuk tugas teknis, dan nilai K tinggi untuk penulisan kreatif.

- **Top-P Sampling**.
yang juga dikenal sebagai **nucleus sampling**, adalah teknik yang digunakan dalam model bahasa untuk menghasilkan teks. Alih-alih mempertimbangkan semua kemungkinan kata berikutnya, teknik ini berfokus pada kumpulan kata terkecil yang probabilitas kumulatifnya melampaui ambang batas 'P'. Berbeda dengan jumlah tetap pada Top-K, Top-P menyesuaikan diri secara dinamis berdasarkan distribusi probabilitas. Nilai rendah (0,1–0,5) menghasilkan keluaran yang terfokus, nilai sedang (0,6–0,9) menyeimbangkan kreativitas dan koherensi, sedangkan nilai tinggi (0,9–0,99) memungkinkan keragaman kreatif.

- **Repetition Penalties**.
Penalti pengulangan mencegah LLM mengulang kata atau frasa dengan cara mengurangi probabilitas pemilihan token yang telah digunakan sebelumnya. Hal ini mencakup penalti frekuensi (yang besarnya bergantung pada jumlah penggunaan) dan penalti keberadaan (yang berlaku sama untuk setiap token yang digunakan). Parameter-parameter ini meningkatkan kualitas keluaran dengan mendorong keragaman kosakata dan mencegah penggunaan frasa yang berlebihan atau repetitif.

### Terminologi Umum
