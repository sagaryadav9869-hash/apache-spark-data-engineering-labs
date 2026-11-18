# PySpark & Spark SQL Data Engineering Practicals

A comprehensive collection of hands-on notebooks and reference guides covering core **Apache Spark** concepts using **PySpark**[cite: 1, 5, 10]. This repository progresses from low-level Resilient Distributed Dataset (RDD) mechanics to structured DataFrame transformations, complex nested types, Spark SQL joins, and performance optimization[cite: 1, 3, 4, 6, 10].

---

## 📂 Repository Contents

| Practical / Module | File(s) | Description | Key Concepts Covered |
| :--- | :--- | :--- | :--- |
| **Prac 1: RDD Fundamentals & Operations** | `DE Pract 1...ipynb`<br>`1. Spark_RDD_Operations.docx`<br>`1b More_Operations.docx` | Core low-level distributed data processing, manual file parsing, and cluster memory management[cite: 1, 2, 5]. | `parallelize()`, `textFile()`, manual CSV parsing, `emptyRDD()`, `reduceByKey()`, `groupByKey()`, `mapValues()`, `repartition()`, `coalesce()`, Broadcast Variables, Accumulators[cite: 1, 2, 5]. |
| **Prac 2: DataFrame Operations** | `Lab 2a DE DataFramOperation.ipynb` | Structured data manipulation, explicit schema enforcement, and reshaping[cite: 6, 7]. | Empty DataFrames/Datasets, `StructType` & `StructField`, nested field flattening, `withColumn()`, `withColumnRenamed()`, `drop()`, `lit()`, type casting (`cast()`), `pivot()` & `stack()` (unpivot)[cite: 6, 7]. |
| **Prac 3: Complex Data Types (Arrays & Maps)** | `Lab 3 DE Array & Map Function.ipynb`<br>`DE 3 Practical...ipynb` | Working with semi-structured and nested collections inside DataFrames[cite: 3, 8]. | `size()`, `array_contains()`, `sort_array()`, `explode()`, `map_keys()`, `map_values()`, `map_entries()`, `map_concat()`, `create_map()`[cite: 3, 8]. |
| **Prac 5: Spark SQL Joins, Schemas & Functions** | `Lab 5 DE Functions.ipynb`<br>`DE 5 Pract Spark SQL Joins...docx` | Relational SQL querying using temporary views, multi-table joins, and built-in SQL functions[cite: 4, 9]. | Explicit `StructType` schemas, `createOrReplaceTempView()`, `INNER`, `LEFT`, `RIGHT`, and `FULL OUTER` joins, `upper()`, `when().otherwise()`, `concat()`, `isNull()`[cite: 4, 9]. |
| **Prac 6: Spark SQL Core APIs & Optimization** | `Lab 6 Spark SQL .ipynb` | Comprehensive DataFrame API transformations, partition-level execution, UDFs, and caching. | `where()`, `filter()`, `distinct()`, `groupBy()`, `union()`, `map()` vs. `mapPartitions()`, `foreach()` vs. `foreachPartition()`, User-Defined Functions (`udf`), `cache()`, and `persist()`[cite: 10]. |

---

## 🛠️ Tech Stack & Environment

* **Engine:** Apache Spark (`3.5.1`)[cite: 3, 5, 9]
* **Language:** Python 3 (PySpark)[cite: 3, 5]
* **Environment:** Google Colab / Databricks / Jupyter Notebook[cite: 3, 4, 5]

---

## 🚀 Getting Started

### Prerequisites
Ensure you have Python 3.8+ and Java (OpenJDK 11) installed if running locally[cite: 9].

### Installation
Install PySpark via pip:
```bash
pip install pyspark
