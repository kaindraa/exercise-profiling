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