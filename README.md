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

## ll. Cara Kerja LLM (Working with LLM)

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

- **AI vs AGI**.
AI (Kecerdasan Buatan) mengacu pada sistem yang dirancang untuk melakukan tugas-tugas tertentu dengan meniru aspek-aspek kecerdasan manusia, seperti pengenalan pola, pengambilan keputusan, dan pemrosesan bahasa. Sistem ini—yang dikenal sebagai "AI sempit" (**narrow AI**)—bersifat sangat khusus; sistem ini unggul dalam bidang tertentu seperti klasifikasi gambar atau algoritma rekomendasi, namun tidak memiliki kemampuan kognitif yang lebih luas. Sebaliknya, AGI (**Artificial General Intelligence** atau Kecerdasan Umum Buatan) adalah bentuk kecerdasan teoretis yang mampu memahami, mempelajari, dan menerapkan pengetahuan pada berbagai macam tugas setara dengan kemampuan manusia. AGI akan memiliki kapasitas untuk berpikir abstrak, bernalar, dan beradaptasi layaknya kemampuan kognitif manusia, sehingga jauh lebih serbaguna dibandingkan sistem AI saat ini. Meskipun teknologi AI masa kini sangat canggih, AGI masih menjadi tujuan jangka panjang yang menghadirkan tantangan kompleks terkait aspek keamanan, etika, dan kelayakan teknis.

- **LLM**.
LLM (**Large Language Model**) adalah AI yang dilatih menggunakan kumpulan data teks berskala besar untuk memahami dan menghasilkan bahasa yang menyerupai bahasa manusia melalui mekanisme prediksi token berikutnya. Meskipun secara bawaan mampu menangani tugas-tugas seperti penerjemahan, peringkasan, dan penulisan, kemampuan lain—seperti menjelajahi web atau mengeksekusi kode—diperoleh melalui lapisan perangkat lunak yang melingkupi model tersebut. Walaupun sangat serbaguna, LLM membutuhkan daya komputasi yang sangat besar dan dapat mencerminkan bias yang terkandung dalam data pelatihannya.

- **Training**
Pelatihan mengacu pada proses mengajarkan model pembelajaran mesin untuk mengenali pola dan membuat prediksi dengan memaparkannya pada suatu dataset. Selama pelatihan, model belajar dari data dengan menyesuaikan parameter internalnya guna meminimalkan kesalahan antara prediksi yang dihasilkannya dan hasil yang sebenarnya. Proses ini melibatkan pemberian data masukan ke model secara berulang, membandingkan keluarannya dengan jawaban yang benar, serta menyempurnakan prediksinya melalui teknik seperti **gradient descent**. Tujuannya adalah agar model mampu melakukan generalisasi dengan baik sehingga dapat membuat prediksi yang akurat terhadap data baru yang belum pernah ditemui sebelumnya.

- **Embedding**.
Embedding adalah representasi vektor yang padat dan kontinu dari data—seperti kata, kalimat, atau gambar—dalam ruang berdimensi lebih rendah. Representasi ini menangkap hubungan semantik dan pola dalam data, di mana item-item yang serupa ditempatkan lebih berdekatan di dalam ruang vektor tersebut. Dalam pembelajaran mesin (machine learning), embedding digunakan untuk mengubah data yang kompleks menjadi bentuk numerik yang lebih mudah diproses oleh model. Sebagai contoh, embedding kata merepresentasikan kata berdasarkan makna dan konteksnya, sehingga memungkinkan model untuk memahami hubungan seperti sinonim atau analogi. Embedding banyak digunakan dalam berbagai tugas seperti pemrosesan bahasa alami (NLP), sistem rekomendasi, dan pengenalan gambar untuk meningkatkan kinerja serta efisiensi model.

- **Vector Databases**.
Basis data vektor adalah sistem khusus yang dirancang untuk menyimpan, mengindeks, dan mengambil vektor berdimensi tinggi—yang sering kali berupa **embedding** yang merepresentasikan data seperti teks, gambar, atau audio. Berbeda dengan basis data tradisional yang menangani data terstruktur, basis data vektor unggul dalam mengelola data tidak terstruktur dengan memungkinkan pencarian kemiripan (**similarity search**) yang cepat, di mana vektor dibandingkan untuk menemukan vektor yang paling mirip dengan kueri. Hal ini menjadikannya komponen penting untuk berbagai tugas seperti pencarian semantik, sistem rekomendasi, dan penemuan konten, yang sangat bergantung pada pemahaman hubungan antar-item. Basis data vektor menggunakan teknik pengindeksan seperti pencarian **approximate nearest neighbor** (ANN) untuk menangani kumpulan data besar secara efisien, sehingga menjamin pengambilan data yang cepat dan akurat bahkan dalam skala besar.

- **Inference**.
Dalam kecerdasan buatan (AI), inferensi mengacu pada proses di mana model pembelajaran mesin yang telah dilatih membuat prediksi atau menarik kesimpulan dari data baru yang belum pernah ditemui sebelumnya. Berbeda dengan tahap pelatihan, inferensi melibatkan penerapan pengetahuan yang telah dipelajari oleh model untuk mengambil keputusan tanpa memerlukan contoh hasil yang spesifik. Pada dasarnya, inferensi adalah kondisi saat model AI sedang beroperasi secara aktif. Sebagai contoh, mobil otonom yang mengenali rambu berhenti di jalan yang belum pernah dilaluinya sebelumnya merupakan bentuk inferensi. Model tersebut mengidentifikasi rambu berhenti di lingkungan baru dan menggunakan pengetahuan yang telah dipelajarinya untuk mengambil keputusan secara waktu nyata (real-time).

- **RAG**
Retrieval-Augmented Generation (RAG) is an AI approach that combines information retrieval with language generation to create more accurate, contextually relevant outputs. It works by first retrieving relevant data from a knowledge base or external source, then using a language model to generate a response based on that information. This method enhances the accuracy of generative models by grounding their outputs in real-world data, making RAG ideal for tasks like question answering, summarization, and chatbots that require reliable, up-to-date information.

- **Agen AI**.
Dalam rekayasa AI, istilah "agen" merujuk pada sistem atau komponen otonom yang mampu mempersepsikan lingkungannya, mengambil keputusan, dan melakukan tindakan untuk mencapai tujuan tertentu. Agen sering kali berinteraksi dengan sistem eksternal, pengguna, atau agen lain untuk melaksanakan tugas-tugas yang kompleks. Tingkat kompleksitasnya pun beragam, mulai dari bot sederhana berbasis aturan hingga agen canggih bertenaga AI yang memanfaatkan model pembelajaran mesin (**machine learning**), pemrosesan bahasa alami (**natural language processing**), dan pembelajaran penguatan (**reinforcement learning**).

- **Context Window**.
Jendela konteks adalah jumlah teks yang dapat diproses oleh LLM dalam satu permintaan, yang diukur dalam satuan token. Jendela ini mencakup **system prompt**, riwayat percakapan, dokumen yang diambil, serta keluaran model itu sendiri saat menghasilkan respons. Jika total konten melampaui batas ini, informasi yang lebih lama atau berprioritas lebih rendah harus dibuang, diringkas, atau dikeluarkan dari konteks aktif. Penyedia model telah memperluas jendela konteks secara signifikan dalam beberapa tahun terakhir, namun jendela yang lebih besar tidak menjamin model akan memanfaatkannya secara optimal.

- **Fine-tuning**.
Fine-tuning melibatkan penggunaan model bahasa besar (LLM) yang telah dilatih sebelumnya dan melatihnya lebih lanjut menggunakan dataset yang lebih kecil dan spesifik untuk tugas tertentu. Proses ini menyesuaikan LLM agar memiliki kinerja lebih baik dalam tugas atau domain tertentu. Namun, fine-tuning dapat memakan banyak sumber daya dan mungkin bukan selalu merupakan pendekatan yang paling efisien. Teknik seperti prompt engineering, retrieval-augmented generation (RAG), atau penggunaan model khusus yang lebih kecil terkadang dapat memberikan hasil yang setara atau bahkan lebih baik dengan kebutuhan komputasi dan data yang lebih rendah.

- **Prompt Engineering**
Rekayasa prompt adalah seni dan ilmu dalam menyusun prompt yang efektif, yaitu instruksi atau masukan yang diberikan kepada model bahasa berskala besar (LLM). Tujuannya adalah merancang prompt yang memancing respons yang diinginkan dari LLM, serta mengarahkannya untuk menghasilkan keluaran yang akurat, relevan, dan kreatif. Proses ini melibatkan pemahaman terhadap kemampuan dan keterbatasan LLM, serta eksperimen dengan berbagai struktur prompt, kata kunci, dan petunjuk kontekstual untuk mencapai hasil yang optimal.

- **Context Engineering**.
Rekayasa konteks adalah praktik merancang dan menyusun informasi yang Anda berikan kepada model AI secara cermat agar model tersebut dapat menjalankan tugasnya dengan lebih baik. Bayangkan hal ini seperti menyiapkan segala sesuatu yang dibutuhkan AI sebelum mulai bekerja—termasuk memberikan instruksi yang tepat, contoh, pengetahuan latar belakang, dan riwayat percakapan—yang semuanya disusun secara cerdas agar model dapat memberikan jawaban terbaik. Alih-alih sekadar mengajukan pertanyaan dan berharap mendapatkan hasil yang bagus, Anda sebenarnya sedang membangun "lingkungan" informasi yang ideal di sekeliling AI untuk mengarahkannya menuju keberhasilan.

## lll. Prompt engineering

**Prompt engineering** adalah praktik merancang input yang efektif untuk **Large Language Model** (Model Bahasa Besar) guna menghasilkan output yang diinginkan. Peta jalan ini mencakup konsep dasar, teknik utama, parameter model, dan metode tingkat lanjut. Ini merupakan keterampilan universal yang dapat dipelajari siapa saja tanpa memerlukan latar belakang pemrograman, namun sangat penting untuk membuka potensi AI di berbagai aplikasi dan bidang.

### Prompt Anatomy

- **Input Format**.
Format input dalam **prompt engineering** berkaitan dengan cara Anda menyusun dan menyajikan **prompt** kepada **large language model** (LLM). Hal ini mencakup pemilihan kata-kata tertentu, tata letak secara keseluruhan, serta penyertaan contoh atau instruksi. Format input yang dirancang dengan baik akan mengarahkan LLM untuk menghasilkan keluaran yang diinginkan, sekaligus meningkatkan relevansi, akurasi, dan konsistensi responsnya. Format input yang efektif merupakan kunci untuk memaksimalkan potensi LLM dalam menjalankan tugas-tugas tertentu.

- **System Prompting**
System prompting menetapkan konteks, tujuan, dan pedoman operasional secara keseluruhan bagi LLM. Hal ini menentukan peran model, batasan perilaku, persyaratan format keluaran, serta mekanisme pengamanan (guardrails). System prompt menyediakan parameter dasar yang memengaruhi seluruh interaksi berikutnya, sehingga memastikan respons AI yang konsisten, terkendali, dan terstruktur sepanjang sesi berlangsung.

- **Role & Behavior**.
Peran & Perilaku, **System prompting** melibatkan penyusunan instruksi yang menentukan peran, kepribadian, dan perilaku keseluruhan model AI saat berinteraksi dengan pengguna. Hal ini memungkinkan Anda membentuk respons AI agar selaras dengan pedoman yang diinginkan—seperti mengadopsi persona tertentu (misalnya, asisten yang suportif atau seorang ahli) ataupun mematuhi batasan terkait nada dan gaya bahasa. Dengan menetapkan aspek-aspek tersebut secara cermat, Anda dapat memengaruhi keluaran AI secara signifikan serta mengarahkannya pada interaksi yang lebih relevan dan efektif.

- **Contextual prompting**.
Prompting kontekstual menyediakan informasi latar belakang spesifik atau detail situasional yang relevan dengan tugas yang sedang dikerjakan, sehingga membantu LLM memahami nuansa dan menyesuaikan responsnya. Berbeda dengan **prompt** sistem atau peran, **prompt** kontekstual memberikan informasi langsung dan spesifik terkait tugas yang bersifat dinamis serta berubah mengikuti situasi. Contohnya: "Konteks: Anda sedang menulis untuk blog tentang gim arkade retro era 80-an. Sarankan 3 topik untuk artikel." Teknik ini memastikan respons yang dihasilkan relevan, akurat, dan disesuaikan dengan konteks spesifik yang diberikan.

- **Constraining Prompts**.
Membatasi prompt sistem melibatkan penetapan batasan dan limitasi secara eksplisit dalam instruksi yang diberikan kepada model bahasa besar (LLM). Teknik ini berfokus untuk mengarahkan LLM agar beroperasi dalam lingkup tertentu, serta mencegahnya menghasilkan respons yang tidak relevan, berbahaya, atau keliru secara faktual dengan menetapkan aturan dan batasan pada perilaku serta format keluarannya.

- **Structured Outputs**.
Output terstruktur dalam **system prompting** mengacu pada perancangan **prompt** yang memandu **Large Language Model** (LLM) untuk menghasilkan respons dalam format yang telah ditentukan sebelumnya, seperti JSON, XML, atau struktur berbasis teks tertentu. Pendekatan ini berfokus pada penyusunan **system prompt** untuk menghasilkan **output** yang dapat diprediksi dan diurai (**parseable**), sehingga memudahkan integrasi respons LLM ke dalam aplikasi dan alur kerja hilir. Dengan memberikan instruksi yang jelas serta contoh struktur **output** yang diinginkan, kita dapat mengekstrak informasi dan mengotomatisasi proses secara andal.

### Prompting Technique

- **Zero-Shot Prompting**.
adalah metode rekayasa prompt yang mengandalkan tahap pra-pelatihan model bahasa besar (LLM) untuk menyimpulkan respons yang tepat. Berbeda dengan metode rekayasa prompt lainnya, seperti few-shot prompting, model tidak diberikan contoh keluaran saat menggunakan teknik zero-shot.

- **Few-Shot Prompting**.
adalah teknik yang digunakan pada model bahasa berskala besar (LLM), di mana Anda menyertakan sejumlah kecil contoh pasangan input-output langsung di dalam prompt itu sendiri. Contoh-contoh ini memperlihatkan perilaku LLM yang diharapkan untuk tugas tertentu. Dengan melihat "beberapa contoh" (few shots) jawaban yang benar tersebut, LLM dapat lebih memahami pola serta menghasilkan respons yang akurat dan relevan untuk input baru yang belum pernah ditemui sebelumnya.

- **ReAct**.
Teknik **prompting** ReAct (Reason and Act) memungkinkan LLM menyelesaikan tugas-tugas kompleks dengan memadukan penalaran dan interaksi dengan perangkat eksternal. Metode ini mengikuti siklus "pemikiran-tindakan-pengamatan" (**thought-action-observation**): menganalisis masalah, melakukan tindakan menggunakan API eksternal, meninjau hasil, serta melakukan iterasi hingga masalah terpecahkan. Pendekatan ini bermanfaat untuk kegiatan penelitian, penyelesaian masalah bertahap, dan tugas-tugas yang membutuhkan data terkini.

### Model Interaction

- **Pemanggilan Fungsi (Function Calling)**
Pemanggilan fungsi memungkinkan **Large Language Models** (LLM) untuk berinteraksi dengan alat dan API eksternal. Alih-alih hanya menghasilkan teks, LLM dapat diinstruksikan untuk mengenali kapan fungsi tertentu perlu dipanggil berdasarkan input pengguna, lalu mengeluarkan argumen yang diperlukan untuk menjalankan fungsi tersebut. Hal ini memungkinkan LLM melakukan tindakan di luar data pelatihannya, seperti mengambil informasi secara **real-time** atau mengotomatiskan tugas.

- **Caching Prompt**.
Caching prompt adalah teknik yang menyimpan hasil dari prompt LLM sebelumnya, sehingga memungkinkan Anda untuk mengambil dan menggunakannya kembali dengan cepat tanpa harus menjalankan ulang prompt tersebut setiap saat. Hal ini dapat meningkatkan efisiensi secara signifikan serta mengurangi biaya saat menangani prompt yang sering digunakan atau membutuhkan sumber daya komputasi yang besar.

- **Respons Streaming**.
adalah salah satu teknik yang dapat digunakan oleh agen AI untuk mengirimkan jawabannya kepada pengguna. Dengan respons streaming, agen mulai mengirimkan kata-kata segera setelah kata-kata tersebut dihasilkan. Pengguna melihat teks muncul dan bertambah di layar secara real-time. Hal ini memberikan kesan cepat serta memungkinkan pengguna untuk menghentikan atau mengubah permintaan lebih awal. Metode ini berguna untuk jawaban yang panjang dan aplikasi berbasis percakapan (chat). Sebaliknya, respons non-streaming menunggu hingga seluruh jawaban siap, lalu mengirimkannya sekaligus. Hal ini membuat kode di sisi klien lebih sederhana serta lebih mudah untuk di-cache atau dicatat (log), namun pengguna harus menunggu lebih lama, terutama untuk output yang berukuran besar.

## lV. Context Engineering

Rekayasa konteks adalah proses menyusun, memformat, dan menyempurnakan informasi yang diberikan kepada **Large Language Model** (LLM) secara strategis untuk memandu penalaran serta meningkatkan akurasi keluarannya. Proses ini melibatkan berbagai teknik—seperti **retrieval-augmented generation** (RAG), penataan **prompt**, dan pemilihan metadata yang relevan—guna memastikan model memiliki pengetahuan latar belakang yang diperlukan untuk menangani tugas-tugas tertentu secara efektif.

### Fundamentals

- **Prompt Engineering vs Context Engineering**.
Rekayasa prompt berfokus pada bagaimana sebuah instruksi dirumuskan untuk mendapatkan respons yang lebih baik dari model. Rekayasa konteks memiliki cakupan yang lebih luas: hal ini berkaitan dengan informasi apa yang sebenarnya diterima oleh model—termasuk sumber, urutan, dan formatnya—di sepanjang alur kerja aplikasi atau agen secara keseluruhan. Prompt yang disusun dengan baik tetap bisa gagal jika model tidak memiliki data, alat, atau riwayat yang tepat untuk menindaklanjutinya. Rekayasa konteks memandang prompt hanya sebagai salah satu bagian dari sistem yang lebih besar, yang juga mencakup pengambilan informasi (retrieval), memori, dan keluaran dari berbagai alat (tools).

- **Apa itu Lapisan Konteks (Context Layer)?**.
Lapisan konteks adalah bagian dari sistem AI yang bertugas mengumpulkan, mengatur, dan menyajikan informasi yang tepat kepada model sebelum model tersebut menghasilkan respons. Lapisan ini berada di antara sumber data mentah—seperti basis data, dokumen, dan API—dengan model itu sendiri, serta menentukan informasi mana yang disertakan dan mana yang tidak. Sebagian tim membangun lapisan ini secara mandiri menggunakan **pipeline** pengambilan data dan penyimpanan memori, sementara tim lain mengandalkan platform konteks khusus. Tujuannya adalah menyediakan informasi yang relevan dan tepercaya bagi model tanpa membebaninya dengan seluruh data yang tersedia.

- **Context Sources**.
Sumber konteks adalah tempat sistem AI mengambil informasi untuk menyusun data yang diproses oleh model pada tahap inferensi. Sumber yang umum digunakan meliputi dokumen dan basis pengetahuan, basis data dan gudang data, repositori kode, alat bantu obrolan dan dukungan, serta keluaran dari pemanggilan alat atau agen lain. Setiap sumber memiliki frekuensi pembaruan, aturan akses, dan format tersendiri; oleh karena itu, penggabungan yang efektif memerlukan normalisasi dan penyaringan sebelum data tersebut sampai ke model. Memilih sumber yang tepat untuk suatu tugas sama pentingnya dengan menentukan seberapa banyak data yang disertakan.

- **MCP**
MCP, atau **Model Context Protocol**, adalah standar terbuka yang memungkinkan aplikasi AI terhubung ke berbagai alat, sumber data, dan layanan eksternal secara konsisten. Alih-alih membuat integrasi khusus untuk setiap alat yang mungkin dibutuhkan oleh sebuah model, pengembang menyediakan akses ke alat tersebut melalui server MCP, sehingga klien yang kompatibel dengan MCP dapat memanggilnya. Hal ini mengurangi jumlah integrasi khusus yang diperlukan seiring dengan semakin banyaknya sistem yang dihubungkan oleh agen AI. MCP diperkenalkan oleh Anthropic dan kini telah diadopsi oleh penyedia model serta pembuat alat lainnya.

- **Context Security**
Keamanan konteks mencakup risiko yang timbul akibat memasukkan konten eksternal atau konten yang tidak tepercaya ke dalam sistem AI. Dokumen, email, atau halaman web yang berbahaya dapat memuat instruksi tersembunyi yang dirancang untuk memanipulasi model—sebuah teknik yang dikenal sebagai **prompt injection**. Kontrol akses yang lemah juga dapat menyebabkan model menampilkan data kepada pengguna yang seharusnya tidak memiliki akses, atau mengakibatkan kebocoran informasi sensitif melalui pemanggilan alat (**tool calls**) dan log. Membangun alur pemrosesan konteks secara aman berarti melakukan validasi sumber, menerapkan pemeriksaan izin sebelum data mencapai model, serta memperlakukan konten yang diambil sebagai data, bukan sebagai instruksi tepercaya.

- **Context Evaluation**.
Evaluasi konteks mengukur apakah informasi yang diberikan kepada model benar-benar membantunya menjalankan tugas dengan baik. Hal ini mencakup pemeriksaan apakah dokumen yang diambil relevan, apakah ada detail penting yang terlewat, serta apakah konten yang tidak relevan atau kedaluwarsa justru menutupi informasi yang penting. Tim menggunakan kombinasi metrik otomatis—seperti presisi dan **recall** pengambilan data—serta tinjauan manual terhadap keluaran model untuk mendeteksi masalah. Tanpa evaluasi ini, alur kerja konteks mungkin tampak lengkap, padahal sebenarnya memberikan materi yang kurang memadai bagi model untuk bekerja.

### Context Engineering Technique

- **RAG dan Dinamis Filter**.
Retrieval-Augmented Generation (RAG) menyempurnakan Large Language Model (LLM) dengan menyediakan informasi yang relevan dan terkini dari sumber eksternal. Filter dinamis adalah teknik yang menyaring informasi yang diambil untuk RAG secara selektif, memastikan LLM hanya menerima konteks yang paling relevan berdasarkan kueri spesifik dan pengguna. Hal ini menghasilkan respons LLM yang lebih akurat, terfokus, dan sesuai dengan konteks.

- **System Memory**.
Sistem memori memungkinkan agen AI untuk menyimpan informasi lintas interaksi, alih-alih harus memulai dari awal setiap kali beroperasi. Memori jangka pendek biasanya mencakup sesi yang sedang berlangsung, sedangkan memori jangka panjang menyimpan fakta, preferensi, atau keputusan masa lalu yang tetap tersimpan melintasi berbagai sesi. Implementasi yang umum dilakukan memadukan penyimpanan vektor untuk pengambilan informasi berbasis makna (semantik) dengan penyimpanan terstruktur untuk fakta-fakta yang memerlukan pengambilan data secara presisi. Perancangan sistem memori yang baik melibatkan keputusan mengenai apa yang perlu disimpan, berapa lama informasi tersebut disimpan, serta bagaimana cara meringkas atau membuang informasi yang tidak lagi berguna.

- **Context Compaction**.
Pemadatan konteks adalah teknik yang digunakan untuk mengurangi panjang konteks yang diberikan kepada model bahasa berskala besar (LLM) tanpa mengorbankan informasi yang relevan. Proses ini bertujuan untuk menghapus informasi yang redundan, tidak relevan, atau kurang penting dari jendela konteks guna menyediakan ruang bagi data tambahan atau meningkatkan efisiensi dan efektivitas pemrosesan LLM. Pemadatan ini dapat melibatkan teknik-teknik seperti peringkasan, penyaringan, atau pemeringkatan ulang informasi konteks.

- Pemrosesan Konteks Panjang
Pemrosesan konteks panjang melibatkan pemberian sejumlah besar teks—seperti keseluruhan basis kode, dokumen panjang, atau riwayat percakapan yang ekstensif—ke dalam model AI dengan cara yang tetap menjaga akurasi model tersebut. Meskipun secara teknis jendela konteks model cukup besar, kinerjanya dapat menurun seiring bertambahnya volume konten; masalah ini sering disebut sebagai **context rot** (penurunan kualitas konteks). Teknik untuk mengatasinya meliputi pemecahan konten menjadi bagian-bagian kecil (**chunking**), pengambilan hanya bagian yang paling relevan, serta peringkasan materi lama alih-alih menyertakannya secara utuh.

- **State & Historical Context**.
Konteks status dan historis mengacu pada pelacakan peristiwa yang telah terjadi dalam suatu percakapan atau alur kerja, sehingga agen dapat bertindak secara konsisten dari waktu ke waktu. Hal ini mencakup urutan pesan pengguna, pemanggilan alat (**tool calls**) beserta hasilnya di masa lalu, serta keputusan apa pun yang telah diambil oleh agen. Tanpa pelacakan ini, agen dapat mengulangi langkah-langkah, memberikan jawaban yang bertentangan dengan jawaban sebelumnya, atau kehilangan jejak dalam tugas yang melibatkan banyak tahapan. Sistem biasanya menyimpan informasi ini sebagai log terstruktur atau objek status yang diperbarui setelah setiap langkah dan dirujuk sebelum langkah berikutnya dilakukan.

- **Multi-agent Context Sharing**.
Berbagi konteks multi-agen mencakup bagaimana agen AI terpisah yang mengerjakan tugas-tugas terkait saling bertukar informasi yang dibutuhkan masing-masing. Saat satu agen mengalihkan tugas ke agen lain, ia harus meneruskan riwayat dan data yang memadai agar agen kedua dapat melanjutkannya tanpa perlu mengulang pekerjaan atau kehilangan detail penting. Mekanisme berbagi yang dirancang dengan buruk dapat menyebabkan agen bekerja dengan gambaran tugas yang usang atau tidak lengkap, sementara pengiriman konteks yang berlebihan dapat memboroskan token dan memperlambat kinerja sistem. Pendekatan yang umum digunakan meliputi penyimpanan memori bersama, pertukaran pesan terstruktur antaragen, serta penggunaan agen koordinator yang menyaring informasi yang diterima oleh setiap sub-agen.

- **Context Isolation**.
Isolasi konteks adalah upaya memisahkan berbagai tugas atau ranah pengetahuan saat bekerja dengan model bahasa besar (LLM). Bayangkan hal ini seperti memberikan ruang khusus bagi setiap tugas. Alih-alih mengandalkan satu LLM besar untuk menangani segalanya sekaligus, Anda menggunakan beberapa "agen" yang lebih kecil; masing-masing agen berfokus pada tugas tertentu dan dilatih menggunakan data khususnya sendiri. Pendekatan ini mencegah informasi yang tidak saling berkaitan saling mengganggu, sehingga menghasilkan keluaran yang lebih akurat dan dapat diandalkan.

- **Context Failure Modes**.
Mode kegagalan konteks adalah berbagai cara umum yang menyebabkan kegagalan pada alur kerja (**pipeline**) konteks dan penurunan kinerja agen. Hal ini mencakup **context poisoning** (peracunan konteks), di mana informasi yang keliru dimasukkan dan dianggap sebagai fakta; **context distraction** (pengalihan perhatian konteks), di mana terlalu banyak konten tidak relevan mengalihkan perhatian model dari hal-hal yang penting; serta **context rot** (penurunan kualitas konteks), di mana akurasi menurun seiring bertambahnya volume konten, bahkan saat masih berada dalam batas kapasitas yang ditetapkan untuk model tersebut. Kegagalan lainnya meliputi penggunaan data usang yang tidak lagi mencerminkan kenyataan serta adanya informasi yang saling bertentangan dari berbagai sumber yang tidak dapat diselaraskan oleh model.

### Tools & Context Warehouse

- **modus**.
adalah **Context Warehouse**—sebuah lapisan infrastruktur yang berada di antara tumpukan data internal perusahaan dan agen AI-nya. Alih-alih mengharuskan tim untuk memodelkan semantik secara manual, modus menggali konteks dari cara organisasi menggunakan datanya saat ini (seperti **query log**, model dbt, dasbor, **pipeline**, kode, dan dokumentasi) serta terus memperbarui pemahaman tersebut seiring dengan perubahan bisnis. Saat **query** dijalankan, sistem ini hanya menyusun konteks yang relevan dengan tugas yang bersangkutan, sehingga agen dapat bekerja berdasarkan informasi yang bermakna (**signal**) dan bukan gangguan yang tidak relevan (**noise**). modus beroperasi secara independen dari **data warehouse**, model, atau platform aplikasi tertentu, serta menyajikan konteks kepada agen yang sudah ada melalui protokol MCP. Penggunaannya umumnya bersifat internal, memungkinkan tim mana pun di perusahaan untuk mendapatkan jawaban AI yang tepercaya mengenai data bisnis mereka sendiri.

- **DataHub**. adalah platform metadata sumber terbuka (**open source**) yang awalnya dikembangkan di LinkedIn untuk melakukan katalogisasi dan pengelolaan data di seluruh organisasi. Platform ini melacak lokasi penyimpanan data, alur perpindahan data antar-sistem, pihak pemilik data, serta cara penggunaannya, sehingga memberikan peta aset data yang dapat ditelusuri bagi tim. Dalam konteks sistem AI, metadata semacam ini membantu menentukan kumpulan data (**dataset**) mana yang tepercaya dan cukup relevan untuk dimasukkan ke dalam model. Karena bersifat sumber terbuka, tim dapat melakukan **self-hosting** dan mengembangkan fitur tambahan secara mandiri, alih-alih bergantung pada vendor layanan terkelola.

- **Atlan**.
adalah platform tata kelola dan katalog data yang membantu organisasi menemukan, mendokumentasikan, dan mengelola aset data mereka di berbagai gudang data (warehouse), alur data (pipeline), dan perangkat BI. Platform ini menyediakan inventaris kumpulan data yang dapat ditelusuri, lengkap dengan informasi mengenai asal-usul (lineage), kepemilikan, dan kualitas, sehingga tim dapat mengetahui sumber data serta tingkat kepercayaannya. Bagi sistem AI, katalog semacam ini dapat berfungsi sebagai sumber konteks yang telah terverifikasi, membantu memastikan bahwa agen mengambil data yang terkini dan dikelola dengan baik, bukan dari sumber yang tidak dapat diandalkan atau data duplikat. Atlan ditawarkan sebagai produk berbasis cloud yang dikelola sepenuhnya (managed service), bukan sebagai perangkat yang di-host secara mandiri (self-hosted).

- **PostHog**.
adalah platform analitik produk yang juga menawarkan apa yang disebutnya sebagai **context warehouse**—sebuah penyimpanan terpadu yang mencakup data peristiwa produk, pemutaran ulang sesi (**session replays**), serta konteks bisnis dari berbagai alat seperti Slack dan tiket dukungan. Alih-alih mengharuskan adanya **pipeline** ETL terpisah untuk memindahkan data antar-sistem, PostHog menyajikan data gabungan ini secara langsung kepada agen AI melalui server MCP-nya, sehingga memungkinkan agen tersebut melakukan kueri terhadap perilaku produk dan konteks bisnis menggunakan antarmuka yang sama dengan yang digunakan oleh manusia.

## V. Types of AI Models (AI Models)

Model AI hadir dalam berbagai bentuk. Model terbuka memberikan akses transparan terhadap arsitektur dan data pelatihannya, sehingga mendorong kolaborasi dan penyesuaian, sedangkan model tertutup menjaga kerahasiaan detail-detail tersebut. Model yang telah dilatih sebelumnya (**pre-trained models**) dilatih menggunakan kumpulan data berskala besar dan dapat disesuaikan lebih lanjut (**fine-tuned**) untuk tugas-tugas spesifik, sehingga menghemat waktu dan sumber daya. Di sisi lain, model yang di-host secara mandiri (**self-hosted models**) menawarkan kendali dan privasi yang lebih besar karena model tersebut diterapkan dan dikelola di infrastruktur Anda sendiri.

### Pre-trained Models

Model pra-latih adalah model **Machine Learning** (ML) yang sebelumnya telah dilatih menggunakan dataset berskala besar untuk menyelesaikan tugas tertentu atau serangkaian tugas. Model-model ini mempelajari pola, fitur, dan representasi dari data pelatihan tersebut, yang kemudian dapat disesuaikan (**fine-tuned**) atau diadaptasi untuk tugas-tugas lain yang terkait. Proses pra-pelatihan ini memberikan titik awal yang baik, sehingga mengurangi jumlah data dan sumber daya komputasi yang diperlukan untuk melatih model baru dari nol.

### Open vs Closed Source Models

Model sumber terbuka tersedia secara bebas untuk kustomisasi dan kolaborasi, sehingga mendorong transparansi dan fleksibilitas; sebaliknya, model sumber tertutup bersifat eksklusif (proprietary), menawarkan kemudahan penggunaan namun membatasi modifikasi dan transparansi.

### Self-Hosted AI Models

Model AI yang dihosting sendiri adalah model pembelajaran mesin (**machine learning**) yang diterapkan dan dijalankan pada infrastruktur Anda sendiri, alih-alih bergantung pada layanan pihak ketiga atau penyedia layanan **cloud**. Hal ini berarti Anda memiliki kendali penuh atas perangkat keras, perangkat lunak, dan data yang digunakan untuk menjalankan model tersebut, sehingga memungkinkan kustomisasi dan keamanan yang lebih baik, serta potensi biaya jangka panjang yang lebih rendah, tergantung pada kebutuhan dan skala spesifik Anda.

## Vl. Choosing the Right Model

Memilih **large language model** (LLM) yang tepat melibatkan pertimbangan berbagai faktor seperti kompleksitas tugas, anggaran, dan kinerja yang diharapkan. Tugas yang lebih sederhana mungkin hanya memerlukan model yang lebih kecil dan efisien, sedangkan masalah yang lebih kompleks akan lebih efektif ditangani oleh model yang lebih besar dengan kapasitas lebih tinggi. Biaya juga merupakan faktor krusial, karena model yang lebih besar umumnya membutuhkan sumber daya komputasi yang lebih besar. Anda juga perlu mengevaluasi akurasi, kecepatan, dan kemampuan model dalam melakukan generalisasi terhadap data baru yang belum pernah ditemui sebelumnya. Pertimbangkan untuk melakukan **fine-tuning** pada model yang sudah ada menggunakan dataset spesifik Anda jika Anda membutuhkan kinerja yang lebih khusus.

### Closed Models

- **Anthropic's Claude**.
Claude dari Anthropic adalah model bahasa AI yang dirancang untuk mendukung sistem AI yang aman dan dapat ditingkatkan skalanya. Dinamai berdasarkan Claude Shannon—tokoh yang dikenal sebagai bapak teori informasi—Claude berfokus pada penggunaan AI yang bertanggung jawab, dengan mengutamakan aspek keamanan, keselarasan dengan niat manusia, serta upaya meminimalkan keluaran yang berbahaya.

- **Google's Gemini**.
Google Gemini adalah model AI canggih besutan Google DeepMind yang dirancang untuk mengintegrasikan pemrosesan bahasa alami dengan kemampuan multimodal, sehingga memungkinkannya memahami dan menghasilkan tidak hanya teks, tetapi juga gambar, video, dan berbagai jenis data lainnya. Model ini memadukan AI generatif dengan kemampuan penalaran, menjadikannya efektif untuk tugas-tugas kompleks yang membutuhkan analisis logis dan pemahaman kontekstual.

- **OpenAI Models (GPT, o-series)**.
Model OpenAI, termasuk GPT dan "seri-o" (seperti Whisper), adalah model AI yang telah dilatih sebelumnya (**pre-trained**) dan ditawarkan oleh OpenAI, serta dapat diakses melalui API mereka. Model GPT unggul dalam tugas-tugas bahasa alami seperti pembuatan teks, penerjemahan, dan penjawaban pertanyaan. Istilah "seri-o" merujuk pada model khusus lainnya dari OpenAI; sebagai contoh, Whisper adalah model transkripsi ucapan-ke-teks (**speech-to-text**).

- **Cohere**.
menawarkan rangkaian model bahasa besar (**large language models** atau LLM) tertutup yang dirancang untuk berbagai tugas pemrosesan bahasa alami (**natural language processing** atau NLP). Model-model ini dapat diakses melalui API serta dilatih dan dikelola oleh Cohere, sehingga pengguna tidak perlu dipusingkan dengan kerumitan melatih dan melakukan **fine-tuning** model sendiri dari nol. Cohere berfokus pada penyediaan solusi NLP tingkat perusahaan yang mengutamakan keamanan, keandalan, dan kemudahan integrasi.

- **Mistral AI**.
adalah perusahaan yang berfokus pada pengembangan model bahasa besar (LLM) dengan bobot terbuka (**open-weight**) untuk menghadirkan solusi AI berkinerja tinggi. Mistral bertujuan menciptakan model yang efisien sekaligus serbaguna, sehingga cocok untuk berbagai tugas pemrosesan bahasa alami, termasuk pembuatan teks, penerjemahan, dan peringkasan. Dengan merilis model berbobot terbuka, Mistral mendorong transparansi dan aksesibilitas, yang memungkinkan pengembang untuk menyesuaikan serta menerapkan solusi AI secara lebih fleksibel dibandingkan dengan model berpemilik (**proprietary**).

### Open Source Models

- **Meta Llama**.
adalah keluarga model bahasa besar (LLM) yang dikembangkan oleh Meta AI. Model-model ini dirancang agar bersifat sumber terbuka (**open-source**) dan mudah diakses, sehingga memungkinkan para peneliti dan pengembang untuk membangun serta bereksperimen dengan LLM tanpa batasan yang biasanya melekat pada model berpemilik (**proprietary**). Model Llama hadir dalam berbagai versi dan ukuran, serta bertujuan untuk menyediakan landasan yang andal dan efisien bagi beragam tugas pemrosesan bahasa alami.

- **DeepSeek**.
merujuk pada keluarga model bahasa besar (LLM) yang dikembangkan oleh DeepSeek AI. Model-model ini dirancang agar tangguh dan efisien, serta mampu menangani berbagai tugas pemrosesan bahasa alami seperti pembuatan teks, penerjemahan, dan penjawaban pertanyaan. Model-model ini disediakan dengan bobot terbuka, yang memungkinkan pengembang dan peneliti untuk menggunakan, mempelajari, serta memodifikasi arsitektur dan parameter model tersebut.

- **Qwen**.
adalah serangkaian model bahasa besar (LLM) yang dikembangkan oleh Alibaba Group. Model-model ini bersifat sumber terbuka (**open-source**), yang berarti kode dan arsitekturnya tersedia untuk publik, sehingga memungkinkan para peneliti dan pengembang untuk menggunakan, mempelajari, serta memodifikasinya sesuai kebutuhan mereka. Model Qwen dirancang untuk menjalankan berbagai tugas pemrosesan bahasa alami—seperti pembuatan teks, penerjemahan, dan penjawaban pertanyaan—serta tersedia dalam beragam ukuran, yang memberikan fleksibilitas berdasarkan sumber daya komputasi dan kebutuhan aplikasi tertentu.

- **Gemma**
adalah keluarga model bahasa besar (**large language models** atau LLM) sumber terbuka yang dikembangkan oleh Google. Model-model ini dirancang agar ringan namun memiliki performa tinggi, sehingga cocok untuk berbagai tugas, termasuk pembuatan teks, penjawaban pertanyaan, dan penyelesaian kode. Model Gemma tersedia dalam berbagai ukuran, yang memungkinkan pengembang untuk memilih model terbaik sesuai dengan batasan sumber daya dan kebutuhan performa mereka.

### Platform & Ecosystem

- **Hugging Face**.
adalah perusahaan AI dan platform sumber terbuka (open-source) terkemuka yang menyediakan berbagai alat, model, dan pustaka untuk pemrosesan bahasa alami (NLP), visi komputer, dan tugas pembelajaran mesin lainnya. Perusahaan ini paling dikenal berkat pustaka "Transformers"-nya, yang mempermudah penggunaan model pra-latih seperti BERT, GPT, T5, dan CLIP, sehingga model-model tersebut dapat digunakan untuk berbagai tugas seperti klasifikasi teks, penerjemahan, peringkasan, dan pengenalan gambar.

- **Hugging Face Tasks**.
Hugging Face mendukung klasifikasi teks, pengenalan entitas bernama (**named entity recognition**), penjawaban pertanyaan, peringkasan, dan penerjemahan. Platform ini juga mencakup tugas multimodal yang melibatkan teks dan gambar, seperti penjawaban pertanyaan visual (VQA) dan pencocokan gambar-teks. Setiap tugas dijalankan oleh berbagai model pra-latih yang dapat diakses dan disesuaikan (**fine-tuned**) dengan mudah melalui pustaka Hugging Face.

- **Hugging Face Hub**.
adalah platform terpusat tempat pengguna dapat menemukan, berbagi, dan berkolaborasi dalam penggunaan model pra-latih, dataset, dan demo untuk pembelajaran mesin (machine learning). Platform ini menampung repositori sumber daya yang sangat luas hasil kontribusi komunitas, sehingga pengguna dapat dengan mudah mengakses dan mengintegrasikan aset-aset tersebut ke dalam proyek AI mereka. Hub ini menyediakan berbagai alat untuk kontrol versi, dokumentasi **model card**, hingga penerapan (**deployment**) berbasis web, yang menyederhanakan proses pemanfaatan model AI yang sudah ada sekaligus memfasilitasi kontribusi kembali kepada komunitas sumber terbuka (**open-source**).

- **Transformers.js**.
adalah pustaka JavaScript yang memungkinkan model transformer—seperti yang berasal dari Hugging Face—untuk dijalankan secara langsung di peramban (browser) atau Node.js tanpa memerlukan layanan cloud. Pustaka ini mendukung berbagai tugas seperti pembuatan teks, analisis sentimen, dan penerjemahan dalam aplikasi web maupun skrip sisi server. Dengan memanfaatkan WebAssembly (Wasm) dan JavaScript yang efisien, Transformers.js menghadirkan kemampuan NLP yang tangguh dengan latensi rendah, privasi yang lebih baik, serta fungsionalitas offline, menjadikannya pilihan ideal untuk aplikasi interaktif real-time yang mengutamakan pemrosesan lokal demi performa dan keamanan.

- **Ollama**.
adalah platform yang menyediakan model bahasa besar (LLM) yang dirancang untuk dijalankan secara lokal pada perangkat pribadi, sehingga memungkinkan penggunaan fitur AI tanpa bergantung pada layanan cloud. Platform ini mengutamakan privasi, performa, dan kemudahan penggunaan dengan memungkinkan pengguna menjalankan model secara langsung di laptop, desktop, atau perangkat edge, serta menghadirkan kemampuan AI yang cepat dan dapat beroperasi secara offline. Melalui alat seperti Ollama SDK, pengembang dapat mengintegrasikan model-model ini ke dalam aplikasi mereka untuk berbagai tugas—seperti pembuatan teks, peringkasan, dan lain-lain—sembari menikmati keuntungan berupa latensi yang lebih rendah, kontrol data yang lebih baik, serta pemrosesan lokal yang lancar.

- **LM Studio**.
adalah aplikasi desktop yang dirancang untuk menemukan, mengunduh, dan menjalankan model bahasa besar (LLM) secara lokal di komputer Anda. Aplikasi ini menyediakan antarmuka yang ramah pengguna untuk bereksperimen dengan berbagai LLM sumber terbuka (open-source) tanpa memerlukan pengetahuan teknis yang mendalam ataupun infrastruktur cloud. Pada dasarnya, aplikasi ini membantu Anda mengelola dan berinteraksi dengan LLM secara langsung di perangkat Anda.

- **OpenRouter**.
berfungsi sebagai API terpadu yang menyediakan akses ke berbagai model bahasa besar (LLM) dari beragam penyedia—seperti OpenAI, Cohere, dan Anthropic—melalui satu platform. Hal ini memungkinkan pengembang untuk beralih antar-model dengan mudah, membandingkan kinerjanya, serta mengoptimalkan aplikasi mereka tanpa perlu mengelola banyak kunci API atau proses integrasi yang rumit. Pada dasarnya, layanan ini menyederhanakan proses eksperimen dan penerapan berbagai model AI.

### APIs & SDKs

- **OpenAI Response API**.
memungkinkan pengembang untuk berinteraksi dengan berbagai model AI yang disediakan oleh OpenAI. API ini menyediakan cara terstruktur untuk mengirimkan permintaan ke model-model tersebut serta menerima teks, kode, atau keluaran lain yang dihasilkan. Anda dapat mengatur berbagai aspek—seperti **prompt**, **temperature**, panjang maksimum, dan parameter lainnya—untuk menyesuaikan respons dengan kebutuhan spesifik Anda. API ini ditujukan untuk menggantikan Assistants API dan Chat Completions API pada proyek-proyek baru di masa mendatang.

- **Claude Messages API**.
menyediakan cara terstruktur untuk berinteraksi dengan model AI Claude. API ini memungkinkan pengembang untuk mengirimkan serangkaian pesan kepada Claude, menyerupai sebuah percakapan. Pesan-pesan tersebut dapat mencakup teks, gambar, dan bahkan data terstruktur, sehingga memungkinkan Anda membangun interaksi yang kompleks serta memperoleh wawasan spesifik dari respons model melalui input dan output yang terstruktur.

- **Google Gemini API**.
memberikan akses terprogram bagi pengembang ke keluarga model AI multimodal Gemini milik Google. API ini memungkinkan aplikasi untuk memahami dan menghasilkan konten yang mencakup teks, gambar, audio, dan video. Pengembang dapat menggunakan API ini untuk membangun berbagai fitur, seperti antarmuka percakapan, alat pembuatan konten, serta sistem yang mampu menganalisis dan merespons data multisensor yang kompleks.

- **Inference SDK**.
Hugging Face Inference SDK adalah alat canggih yang memungkinkan pengembang untuk dengan mudah mengintegrasikan dan menjalankan inferensi pada model bahasa besar (**large language models**) yang di-host di Hugging Face Hub. Dengan menggunakan InferenceClient, pengguna dapat melakukan panggilan API ke berbagai model untuk tugas-tugas seperti pembuatan teks, pembuatan gambar, dan banyak lagi. SDK ini mendukung operasi sinkron maupun asinkron, sehingga kompatibel dengan alur kerja yang sudah ada.

- **OpenAI-compatible APIs**.
API yang kompatibel dengan OpenAI adalah antarmuka yang meniru struktur dan fungsionalitas API OpenAI. API ini memungkinkan pengembang untuk beralih antar-model bahasa atau penyedia layanan yang berbeda dengan perubahan kode yang minimal. Hal ini sangat berguna untuk menguji berbagai model, mengurangi ketergantungan pada satu vendor (**vendor lock-in**), atau membangun mekanisme cadangan (**fallback**) jika terjadi gangguan layanan.

## Embeddings & Vector Database

**Apa itu Embedding?**
Embedding adalah representasi vektor numerik yang padat dari data—seperti kata, kalimat, gambar, atau audio—yang menangkap makna semantik serta hubungan antar-data tersebut. Dengan mengubah data menjadi vektor berukuran tetap, embedding memungkinkan model pembelajaran mesin (machine learning) untuk memproses dan memahami data secara lebih efektif. Sebagai contoh, embedding kata merepresentasikan kata-kata yang serupa dengan vektor yang juga serupa, sehingga memungkinkan dilakukannya tugas-tugas seperti pencarian semantik, sistem rekomendasi, dan klasterisasi. Embedding mempermudah proses perbandingan, pencarian, dan analisis data kompleks yang tidak terstruktur dengan cara memetakan item-item yang serupa agar berdekatan satu sama lain dalam ruang berdimensi tinggi.

### Use Case for Embeddings

- **Semantic Search**
Embedding digunakan untuk pencarian semantik dengan cara mengubah teks—seperti kueri dan dokumen—menjadi vektor berdimensi tinggi yang menangkap makna serta konteks yang mendasarinya, bukan sekadar kata-kata persis. Embedding ini merepresentasikan hubungan semantik antar-kata atau frasa, sehingga memungkinkan sistem untuk memahami maksud kueri dan mengambil informasi yang relevan, meskipun istilah yang digunakan tidak sama persis.

- **Data Classification**.
Setelah data diubah menjadi **embedding**, algoritma klasifikasi—seperti jaringan saraf (**neural network**) atau model regresi logistik—dapat dilatih menggunakan **embedding** tersebut untuk mengelompokkan data ke dalam berbagai kategori. Keunggulan penggunaan **embedding** terletak pada kemampuannya menangkap hubungan dan kemiripan mendasar antar titik data, bahkan ketika data mentahnya bersifat kompleks atau berdimensi tinggi; hal ini meningkatkan akurasi klasifikasi dalam berbagai tugas seperti klasifikasi teks, kategorisasi gambar, dan sistem rekomendasi.

- **Recommendation Systems**.
Dalam konteks **embedding**, sistem rekomendasi menggunakan representasi vektor untuk menangkap kemiripan antar-item, seperti produk atau konten. Dengan mengubah item dan preferensi pengguna menjadi **embedding**, sistem ini dapat mengukur tingkat keterkaitan antar-item berdasarkan kedekatan vektor, sehingga memungkinkan rekomendasi produk atau konten serupa berdasarkan interaksi pengguna di masa lalu. Pendekatan ini meningkatkan akurasi dan efisiensi rekomendasi dengan memfasilitasi perbandingan data yang kompleks secara bermakna dan dapat diskalakan.

- **Anomaly Detection**.
Deteksi anomali menggunakan **embedding** bekerja dengan cara mengubah data—seperti teks, gambar, atau data deret waktu—menjadi representasi vektor yang menangkap pola serta hubungan di dalamnya. Dalam ruang berdimensi tinggi ini, titik-titik data yang serupa ditempatkan berdekatan, sedangkan anomali tampak menonjol karena menyimpang secara signifikan dari distribusi umum. Pendekatan ini sangat efektif untuk mendeteksi **outlier** dalam berbagai tugas seperti deteksi penipuan, keamanan jaringan, dan pengendalian kualitas.

**Embedding Model**.
mengubah data, seperti teks atau gambar, menjadi representasi numerik yang disebut embedding. Embedding ini menangkap makna semantik dan hubungan antar-data dalam ruang vektor. Dengan merepresentasikan data sebagai vektor, kita dapat melakukan operasi matematika untuk menentukan tingkat kemiripan, mengelompokkan item yang saling terkait, serta memasukkan data tersebut ke dalam model pembelajaran mesin.

### Proprietary Model (Model Eksklusif)

- **OpenAI Embeddings API**.
menyediakan cara praktis untuk mengubah teks menjadi representasi vektor numerik yang disebut **embedding**. **Embedding** ini menangkap makna semantik teks, sehingga memungkinkan Anda melakukan berbagai tugas seperti pencarian semantik, pengelompokan (**clustering**), dan perbandingan kemiripan dengan menganalisis hubungan antarvektor tersebut. API ini menyederhanakan proses pembuatan **embedding** dengan menyembunyikan kompleksitas terkait pelatihan dan pengelolaan model **embedding**.

- **Gemini Embedding**.
API Gemini menyediakan metode untuk mengubah teks, gambar, atau jenis data lainnya menjadi representasi vektor numerik yang disebut **embedding**. **Embedding** ini menangkap makna semantik dan hubungan antarberbagai informasi, sehingga memungkinkan dilakukannya pencarian kemiripan, pengelompokan (**clustering**), dan tugas pembelajaran mesin lainnya secara efisien. Model-model eksklusif ini ditawarkan sebagai layanan—sering kali melalui API—serta memerlukan pembayaran atau langganan.

- **Cohere Embeddings**.
Cohere menawarkan **embedding** teks yang tangguh, yaitu representasi numerik dari data teks. **Embedding** ini menangkap makna semantik dari kata, kalimat, dan dokumen, sehingga memungkinkan model AI untuk memahami hubungan serta melakukan berbagai tugas seperti pencarian kemiripan, pengelompokan (**clustering**), dan temu kembali informasi (**information retrieval**). Model **embedding** Cohere dirancang untuk memberikan akurasi dan kinerja tinggi dalam berbagai aplikasi pemrosesan bahasa alami (**natural language processing**).

### Open Source Models

- **Sentence Transformers**.
adalah jenis model yang dirancang untuk menghasilkan **embedding** berkualitas tinggi bagi kalimat, sehingga mampu menangkap makna semantik dari teks. Berbeda dengan **embedding** kata tradisional yang merepresentasikan kata-kata secara individual, Sentence Transformers memahami konteks kalimat secara utuh; hal ini menjadikannya ideal untuk tugas-tugas yang memerlukan pemahaman kemiripan semantik, seperti pengelompokan kalimat, pencarian semantik, dan deteksi parafrasa. Dibangun di atas model **transformer** seperti BERT dan RoBERTa, model ini mengubah kalimat menjadi vektor padat (**dense vectors**), di mana kalimat-kalimat yang serupa ditempatkan lebih berdekatan dalam ruang vektor.

- **Model on Hugging Face**.
Model **embedding** digunakan untuk mengubah data mentah—seperti teks, kode, atau gambar—menjadi vektor berdimensi tinggi yang menangkap makna semantik. Representasi vektor ini memungkinkan sistem AI untuk membandingkan, mengelompokkan, dan mengambil informasi berdasarkan kemiripan, bukan sekadar kecocokan persis. Hugging Face menyediakan beragam model **embedding** yang telah dilatih sebelumnya (**pretrained**), yang umum digunakan untuk berbagai tugas seperti pencarian semantik, sistem rekomendasi, deteksi duplikat, dan **retrieval-augmented generation** (RAG). Model-model ini dapat diakses melalui pustaka seperti **transformers** atau **sentence-transformers**, sehingga memudahkan pembuatan **embedding** berkualitas tinggi untuk aplikasi tujuan umum maupun aplikasi yang dirancang untuk tugas spesifik.

- **Jina AI**.
Jina Embeddings adalah rangkaian model **embedding** berkinerja tinggi, sumber terbuka (**open-source**), multibahasa, dan multimodal yang dikembangkan oleh Jina AI. Model-model ini mengubah data teks dan visual (seperti gambar dan grafik) menjadi vektor numerik padat untuk keperluan pencarian semantik, RAG, dan aplikasi AI. Fitur-fitur utamanya mencakup dukungan untuk konteks panjang (hingga 32 ribu token), kemampuan multi-tugas, serta versi khusus untuk **text-to-image** dan pengambilan kode (**code retrieval**).

**Vector Databases**.
Basis data vektor adalah sistem yang dirancang khusus untuk menyimpan, mengindeks, dan mengambil vektor berdimensi tinggi—yang sering kali digunakan sebagai **embedding** untuk data seperti teks, gambar, atau audio. Berbeda dengan basis data tradisional, sistem ini unggul dalam mengelola data tidak terstruktur dengan memungkinkan pencarian kemiripan (**similarity search**) yang cepat, di mana vektor dibandingkan untuk menemukan kecocokan terdekat. Hal ini menjadikannya komponen penting untuk berbagai tugas seperti pencarian semantik, sistem rekomendasi, dan penemuan konten. Dengan memanfaatkan teknik seperti pencarian **approximate nearest neighbor** (ANN), basis data vektor mampu menangani kumpulan data berskala besar secara efisien, sehingga menjamin pengambilan data yang cepat dan akurat.

**Tujuan dan Fungsionalitas**.
Basis data vektor dirancang untuk menyimpan, mengelola, dan mengambil vektor berdimensi tinggi (embedding) yang dihasilkan oleh model AI. Tujuan utamanya adalah melakukan pencarian kemiripan yang cepat dan efisien, sehingga memungkinkan aplikasi menemukan titik data yang secara semantik atau visual mirip dengan kueri tertentu. Berbeda dengan basis data tradisional yang menangani data terstruktur, basis data vektor unggul dalam mengelola data tidak terstruktur—seperti teks, gambar, dan audio—dengan mengubahnya menjadi representasi vektor padat. Basis data ini menggunakan teknik pengindeksan, seperti algoritma **approximate nearest neighbor** (ANN), untuk menelusuri kumpulan data berskala besar secara cepat dan menyajikan hasil yang relevan. Basis data vektor sangat penting bagi aplikasi seperti sistem rekomendasi, pencarian semantik, dan penemuan konten, di mana kemampuan untuk memahami serta mengambil item yang serupa menjadi hal yang krusial.

### Vector DBs Populer

- **Chroma**.
adalah basis data vektor sumber terbuka (**open-source**) dan basis data **embedding** yang dirancang secara khusus untuk AI (**AI-native**), yang ditujukan untuk menangani serta menyimpan **embedding** dan vektor semantik berskala besar. Chroma digunakan dalam berbagai aplikasi yang membutuhkan pencarian kemiripan yang cepat dan efisien, seperti pemrosesan bahasa alami (NLP), pembelajaran mesin (ML), serta sistem AI yang mengolah teks, gambar, dan jenis data berdimensi tinggi lainnya.

- **Pinecone**.
adalah basis data vektor terkelola yang dirancang untuk pencarian kemiripan dan pengambilan data berdimensi tinggi—seperti **embedding**—secara efisien dan **real-time**. Layanan ini memungkinkan pengembang untuk menyimpan, mengindeks, dan melakukan kueri terhadap representasi vektor, sehingga mempermudah pembuatan aplikasi seperti sistem rekomendasi, pencarian semantik, dan penemuan konten berbasis AI. Pinecone bersifat skalabel, mampu menangani kumpulan data berskala besar, serta menyediakan pencarian yang cepat dengan latensi rendah melalui teknik pengindeksan yang dioptimalkan.

- **Weaviate**.
adalah basis data vektor sumber terbuka (**open-source**) yang memungkinkan pengguna untuk menyimpan, mencari, dan mengelola vektor berdimensi tinggi; sistem ini sering digunakan untuk tugas-tugas seperti pencarian semantik dan sistem rekomendasi. Weaviate memfasilitasi pencarian kemiripan yang efisien dengan mengubah data (seperti teks, gambar, atau audio) menjadi **embedding** dan mengindeksnya untuk pengambilan data yang cepat. Selain itu, Weaviate mendukung integrasi sumber data serta skema eksternal, sehingga memudahkan penggabungan data terstruktur dan tidak terstruktur.

- **FAISS**.
(Facebook AI Similarity Search) adalah pustaka yang dikembangkan oleh Facebook AI untuk pencarian kemiripan dan pengelompokan vektor padat (**dense vectors**) secara efisien, yang sangat berguna untuk dataset berskala besar. Pustaka ini dioptimalkan untuk menangani **embedding** (representasi vektor) dan memungkinkan pencarian tetangga terdekat (**nearest neighbor search**) yang cepat, sehingga Anda dapat mengambil item serupa dari kumpulan vektor yang besar berdasarkan metrik jarak atau kemiripan, seperti **cosine similarity** atau jarak Euclidean. FAISS banyak digunakan dalam berbagai aplikasi seperti temu balik gambar dan teks, sistem rekomendasi, dan sistem pencarian berskala besar yang memanfaatkan **embedding** untuk merepresentasikan item. FAISS menawarkan berbagai metode pengindeksan dan mampu menangani hingga miliaran vektor, menjadikannya alat yang ampuh untuk menyelesaikan masalah pencarian kemiripan berskala besar secara **real-time** dan efisien.

- **LanceDB**.
adalah basis data vektor yang dirancang untuk penyimpanan, pengambilan, dan pengelolaan **embedding** secara efisien. Sistem ini memungkinkan pengguna melakukan pencarian kemiripan (**similarity search**) dengan cepat, yang sangat berguna dalam aplikasi seperti sistem rekomendasi, pencarian semantik, dan pengambilan konten berbasis AI. LanceDB berfokus pada skalabilitas dan kecepatan, sehingga memungkinkan pengindeksan dan kueri kumpulan data **embedding** berskala besar secara cepat—hal yang krusial bagi aplikasi AI waktu nyata (**real-time**). LanceDB terintegrasi dengan baik dalam alur kerja pembelajaran mesin (**machine learning**), mempermudah penerapan model yang mengandalkan pemrosesan data berbasis vektor, serta membantu mengelola kompleksitas penanganan data vektor berdimensi tinggi secara efisien.

- **Qdrant**.
adalah basis data vektor sumber terbuka (**open-source**) yang dirancang untuk pencarian kemiripan yang efisien dan pengambilan data secara **real-time**. Basis data ini memiliki spesialisasi dalam menyimpan dan mengindeks vektor berdimensi tinggi (**embedding**) guna memungkinkan pencarian yang cepat dan akurat pada kumpulan data berskala besar. Qdrant sangat cocok untuk aplikasi seperti sistem rekomendasi, pencarian semantik, dan penemuan konten berbasis AI, di mana kemampuan menemukan item serupa dengan cepat merupakan hal yang krusial. Qdrant mendukung pemfilteran tingkat lanjut, pengindeksan yang dapat diskalakan, serta pembaruan **real-time**, sehingga mudah diintegrasikan ke dalam alur kerja **machine learning**.

- **Supabase**.
Vector adalah ekstensi dari platform Supabase yang dirancang khusus untuk aplikasi AI dan **machine learning** yang memerlukan operasi vektor. Fitur ini memanfaatkan ekstensi pgvector pada PostgreSQL untuk menyediakan penyimpanan vektor yang efisien serta kemampuan pencarian kemiripan (**similarity search**). Hal ini menjadikan Supabase Vector sangat berguna bagi aplikasi yang melibatkan **embedding**, pencarian semantik, dan sistem rekomendasi. Dengan Supabase Vector, pengembang dapat menyimpan dan melakukan kueri data vektor berdimensi tinggi bersamaan dengan data relasional biasa, semuanya dalam satu basis data PostgreSQL yang sama.

- **MongoDB Atlas**.
traditionally known for its document database capabilities, now includes vector search functionality, making it a strong option as a vector database. This feature allows developers to store and query high-dimensional vector data alongside regular document data. With Atlas’s vector search, users can perform similarity searches on embeddings of text, images, or other complex data, making it ideal for AI and machine learning applications like recommendation systems, image similarity search, and natural language processing tasks. The seamless integration of vector search within the MongoDB ecosystem allows developers to leverage familiar tools and interfaces while benefiting from advanced vector-based operations for sophisticated data analysis and retrieval.

### Mengimplementasikan Pencarian Vektor

- **Indexing Embeddings (Pengindeksan Embedding)**.
Embedding disimpan dalam basis data vektor dengan terlebih dahulu mengubah data—seperti teks, gambar, atau audio—menjadi vektor berdimensi tinggi menggunakan model pembelajaran mesin. Vektor-vektor ini, yang juga disebut sebagai embedding, menangkap hubungan semantik dan pola yang terkandung dalam data tersebut. Setelah dihasilkan, setiap embedding diindeks dalam basis data vektor bersama dengan metadata terkaitnya, seperti data asli (misalnya, teks atau gambar) atau sebuah pengenal (identifier). Basis data vektor kemudian mengatur embedding-embedding ini untuk mendukung pencarian kemiripan yang efisien, biasanya dengan menggunakan teknik seperti pencarian **approximate nearest neighbor** (ANN).

- **Performing Similarity Search (Melakukan Pencarian Kemiripan)**.
Dalam pencarian kemiripan, proses dimulai dengan mengubah kueri pengguna (seperti potongan teks atau gambar) menjadi **embedding**—yaitu representasi vektor yang menangkap makna semantik dari kueri tersebut. **Embedding** ini dihasilkan menggunakan model yang telah dilatih sebelumnya, seperti BERT untuk teks atau jaringan saraf (**neural network**) untuk gambar. Setelah kueri diubah menjadi vektor, vektor tersebut dibandingkan dengan **embedding** yang tersimpan di dalam basis data vektor.

**RAGs**. Implementasi Retrieval-Augmented Generation (RAG) menggabungkan pengambilan informasi dengan pembuatan bahasa untuk menghasilkan respons yang lebih akurat dan kontekstual. Metode ini menggunakan dua komponen: **retriever** (pengambil informasi) yang menelusuri basis data untuk menemukan informasi relevan, dan **generator** (pembuat respons) yang menyusun jawaban berdasarkan data yang telah diperoleh. Implementasi RAG melibatkan penggunaan model pengambilan informasi (misalnya, **embedding** dan pencarian vektor) bersama dengan model bahasa generatif (seperti GPT). Prosesnya dimulai dengan mengubah kueri menjadi **embedding**, mengambil dokumen relevan dari basis data vektor, lalu memasukkannya ke dalam model bahasa, yang kemudian menghasilkan respons yang koheren dan kaya informasi. Pendekatan ini mendasarkan keluaran pada data dunia nyata, sehingga menghasilkan jawaban yang lebih andal dan terperinci.

**RAG Usecases**.
Retrieval-Augmented Generation (RAG) meningkatkan kemampuan aplikasi seperti chatbot, layanan pelanggan, dan peringkasan konten dengan memadukan pengambilan informasi serta pembuatan bahasa. Teknologi ini mengambil data relevan dari basis pengetahuan dan memanfaatkannya untuk menghasilkan respons yang akurat dan kontekstual, sehingga ideal untuk tugas-tugas seperti menjawab pertanyaan, pembuatan dokumen, dan pencarian semantik. Kemampuan RAG untuk mendasarkan hasil keluarannya pada informasi dunia nyata menghasilkan keluaran yang lebih andal dan informatif, sekaligus meningkatkan pengalaman pengguna di berbagai bidang.

**RAG vs. Fine-tuning**.
RAG (Retrieval-Augmented Generation) dan fine-tuning adalah dua pendekatan untuk meningkatkan kemampuan model bahasa, namun keduanya berbeda dalam hal metodologi dan kasus penggunaannya. Fine-tuning melibatkan pelatihan model yang sudah terlatih sebelumnya (pre-trained model) menggunakan dataset khusus untuk menyesuaikannya dengan tugas tertentu; hal ini membuat model lebih akurat dalam konteks tersebut, namun pengetahuannya terbatas pada informasi yang ada dalam data pelatihan. Di sisi lain, RAG menggabungkan pengambilan informasi secara real-time dengan proses pembuatan teks (generasi), sehingga memungkinkan model mengakses data eksternal terkini dan menghasilkan respons yang relevan secara kontekstual. Jika fine-tuning ideal untuk tugas-tugas khusus yang bersifat statis, maka RAG lebih cocok untuk tugas-tugas dinamis yang membutuhkan respons berbasis fakta secara real-time.

