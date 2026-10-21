# JOBSHEET 7 - LOOPS 1

**Identitas Mahasiswa:**
* **Nama:** Datu Ayu Fitria Ceasa
* **NIM:** 264107020087
* **Kelas / No. Presensi:** 1I / 06

---

## 1: OBJECTIVES

1. Students are able to explain the syntax for writing loop programs (for, while, and do while). 
2. Students are able to implement loop flowcharts using the Java programming 
language. 

---

## 2: Practical Exercises

### 2.1 Experiment 1: Student Grades Case Study in SIAKAD – FOR Loop

#### 2.1.1 Java Code
```java
import java.util.Scanner;

public class SiakadFor06 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double score, highest = 0, lowest = 100;
        for (int i = 1; i <= 10; i++) { 
            System.out.print("Enter score for student " + i + ": "); 
            score = sc.nextDouble(); 
            if (score > highest) { 
                highest = score; 
            } 
            if (score < lowest) { 
                lowest = score; 
            } 
        } 
        System.out.println("Highest score: " + highest); 
        System.out.println("Lowest score: " + lowest); 
    }
}
```

#### 2.1.2 Screenshot Output
Berikut adalah contoh tampilan *output* setelah program dijalankan:

![Example Image of Experiment 1 Output](/StudentScore.png)

#### 2.1.3 Questions
* **Question 1:** Apa fungsi dari perintah `if`?
  * **Answer:** Identify and indicate each component of the FOR loop in the program code of Experiment 1! 
* **Question 2:** Why is the variable highest initialized to 0 and the variable lowest initialized to 100? What happens if highest is initialized to 100 and lowest is initialized to 0? 
  * **Answer:** Program akan melewati blok `if` dan mengeksekusi blok `else` (jika ada).
* **Question 3:** Explain the function and workflow of the following code snippet!
![](/StudentScore.png)
  * **Answer:** Program akan melewati blok `if` dan mengeksekusi blok `else` (jika ada).
* **Question 4:** Modify the program to count how many students pass and how many students fail, based on the passing threshold (minimum score of 60). Display the number of students who pass and fail after displaying the highest and lowest scores!  
  * **Answer:** Program akan melewati blok `if` dan mengeksekusi blok `else` (jika ada).

---

### 2.2 Percobaan 2: Penerapan Structure SWITCH-CASE

Paragraf ini menjelaskan ringkasan Percobaan 2. Percobaan ini berfokus pada penggunaan `switch-case` untuk memilih menu atau opsi berdasarkan nilai yang bersifat spesifik.

#### 2.2.1 Tabel Pengujian Parameter Output

Berikut adalah hasil uji coba program dengan beberapa variasi masukan *dummy*:

| No | Input Parameter | Output yang Dihasilkan | Status Eksekusi |
| :---: | :--- | :--- | :---: |
| 1 | `Case 1` | "Pilihan 1 Dipilih" | Valid |
| 2 | `Case 2` | "Pilihan 2 Dipilih" | Valid |
| 3 | `Default` | "Pilihan Tidak Tersedia" | Invalid |

---

## 3: TUGAS MANDIRI

Berikut adalah daftar tugas yang dikerjakan pada Jobsheet ini:

- [x] **Tugas 1:** Mengubah struktur `if-else` menjadi *Ternary Operator*.
- [x] **Tugas 2:** Membuat program berdasarkan *Flowchart* penentuan SKS.
- [ ] **Tugas 3:** Mengimplementasikan studi kasus parkir & antrean.

### 3.1 Implementasi Kode Tugas

```java
// Contoh Kode Program Tugas Mandiri
public class TugasMandiri {
    public static void main(String[] args) {
        int sks = 20;
        String status = (sks <= 24) ? "KRS Valid" : "Melebihi Batas";
        System.out.println(status);
    }
}
```

---

## 4: KESIMPULAN

Tuliskan paragraf kesimpulan di sini. Secara singkat, struktur pemilihan sangat penting digunakan untuk mengatur alur jalannya program (*flow control*) berdasarkan variabel atau pilihan yang ditentukan oleh pengguna.
