# Module 5: Java Profiling

---
### Kaindra Rizq Sachio
### 2306274964   
### CSCM602223 - Pemrograman Lanjut

---

# JMeter GUI Test Plan Results 

## GUI Before Profiling
1. `/all-students` endpoint:  
   ![Test Plan 1](./test_results_image/gui_test_plan_1.png)

2. `/all-student-name` endpoint:  
   ![Test Plan 2](./test_results_image/gui_test_plan_2.png)

3. `/highest-gpa` endpoint:  
   ![Test Plan 3](./test_results_image/gui_test_plan_3.png)

## CLI Before Profiling

1. `/all-students` endpoint:  
   ![Test Plan CLI 1](./test_results_image/cli_test_plan_1.png)

2. `/all-student-name` endpoint:  
   ![Test Plan CLI 2](./test_results_image/cli_test_plan_2.png)

3. `/highest-gpa` endpoint:  
   ![Test Plan CLI 3](./test_results_image/cli_test_plan_3.png)

## GUI After Profiling

1. `/all-students` endpoint:  
   ![Test Plan 1 Post](./test_results_image/gui_test_plan_1_post.png)

2. `/all-student-name` endpoint:  
   ![Test Plan 2 Post](./test_results_image/gui_test_plan_2_post.png)

3. `/highest-gpa` endpoint:  
   ![Test Plan 3 Post](./test_results_image/gui_test_plan_3_post.png)

## CLI After Profiling

1. `/all-students` endpoint:  
   ![Test Plan CLI 1 Post](./test_results_image/cli_test_plan_1_post.png)

2. `/all-student-name` endpoint:  
   ![Test Plan CLI 2 Post](./test_results_image/cli_test_plan_2_post.png)

3. `/highest-gpa` endpoint:  
   ![Test Plan CLI 3 Post](./test_results_image/cli_test_plan_3_post.png)

## Conclusion


Perbandingan Hasil Pengujian

| Endpoint           | Sebelum (ms) | Sesudah (ms) | Peningkatan (%)          |
|-------------------|-------------|-------------|--------------------------|
| **/all-students**    | 256,547      | 15,685       | **↓ 93.89% lebih cepat** |
| **/all-student-name** | 6,202        | 4,456        | **↓ 28.15% lebih cepat** |
| **/highest-gpa**      | 217          | 181          | **↓ 16.59% lebih cepat** |

Setelah dilakukan proses profiling dan optimasi, hasil pengujian menggunakan JMeter menunjukkan bahwa semua endpoint mengalami peningkatan performa. Peningkatan paling signifikan terjadi pada endpoint /all-students, yang mengalami pengurangan waktu eksekusi hingga 93,89%, membuktikan bahwa optimasi telah berhasil mengatasi bottleneck utama program dan meningkatkan efisiensi pemrosesan data secara keseluruhan.

# Reflection

> What is the difference between the approach of performance testing with JMeter and profiling with IntelliJ Profiler in the context of optimizing application performance?

JMeter digunakan untuk menguji performa aplikasi dalam skenario nyata, menilai throughput, latensi, dan respons API dalam tinggi. Sementara itu, IntelliJ Profiler lebih fokus pada analisis internal kode.

> How does the profiling process help you in identifying and understanding the weak points in your application?

Profiling membantu dalam mendeteksi area kode yang menggunakan sumber daya berlebihan atau eksekusi yang lambat. Dengan informasi ini, optimasi dapat difokuskan pada bagian yang paling berpengaruh terhadap kinerja keseluruhan.

> Do you think IntelliJ Profiler is effective in assisting you to analyze and identify bottlenecks in your application code?

IntelliJ Profiler sangat berguna dalam memberikan informasi mengenai penggunaan CPU, memori, dan metode yang paling sering dipanggil. Dengan alat ini, developer dapat lebih mudah menemukan serta memperbaiki bagian kode yang menghambat performa aplikasi.

> What are the main challenges you face when conducting performance testing and profiling, and how do you overcome these challenges?

Salah satu tantangan utama adalah mendapatkan hasil yang konsisten antara pengujian performa dan profiling dalam berbagai kondisi sistem. Untuk mengatasi hal ini, pengujian dilakukan secara berulang dengan parameter yang dikontrol agar hasilnya dapat dianalisis secara lebih akurat.

> What are the main benefits you gain from using IntelliJ Profiler for profiling your application code?

IntelliJ Profiler mempercepat proses identifikasi bottleneck dengan analisis otomatis terhadap penggunaan. Selain itu, visualisasi yang disediakan memudahkan saya untuk menganalisis performa

> How do you handle situations where the results from profiling with IntelliJ Profiler are not entirely consistent with findings from performance testing using JMeter?

Jika terdapat perbedaan antara hasil profiling dengan IntelliJ Profiler dan pengujian performa menggunakan JMeter, perlu dilakukan analisis lebih lanjut terkait faktor eksternal seperti kondisi lingkungan atau mekanisme caching. Pengujian ulang dengan skenario berbeda dapat membantu memastikan keakuratan hasil yang diperoleh.

> What strategies do you implement in optimizing application code after analyzing results from performance testing and profiling? How do you ensure the changes you make do not affect the application's functionality?

Setelah analisis pengujian performa dan profiling, strategi optimasi dilakukan dengan meningkatkan efisiensi algoritma dan mengoptimalkan query database. Setelah itu, dilakukan pengujian perbandingan hasil sebelum dan sesudah optimasi.
