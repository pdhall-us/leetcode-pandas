# 595. Big Countries

**Difficulty:** 🟢 Easy

**Topics:** Pandas, Data Filtering, Boolean Indexing, Column Selection

**Problem Link:** [595. Big Countries](https://leetcode.com/problems/big-countries/)

---

## 📝 Problem Statement

Table: `World`

| Column Name | Type |
|---|---|
| name | varchar |
| continent | varchar |
| area | int |
| population | int |
| gdp | bigint |

`name` is the primary key (column with unique values) for this table.

Each row of this table gives information about the name of a country, the continent to which it belongs, its area, the population, and its GDP value.

A country is **big** if:

- It has an area of at least three million (i.e., `3000000 km2`), or
- It has a population of at least twenty-five million (i.e., `25000000`).

Write a solution to find the name, population, and area of the **big countries**.

Return the result table in **any order**.

## 📊 Example 1

**Input:**

World table:

| name | continent | area | population | gdp |
|---|---|---:|---:|---:|
| Afghanistan | Asia | 652230 | 25500100 | 20343000000 |
| Albania | Europe | 28748 | 2831741 | 12960000000 |
| Algeria | Africa | 2381741 | 37100000 | 188681000000 |
| Andorra | Europe | 468 | 78115 | 3712000000 |
| Angola | Africa | 1246700 | 20609294 | 100990000000 |

**Output:**

| name | population | area |
|---|---:|---:|
| Afghanistan | 25500100 | 652230 |
| Algeria | 37100000 | 2381741 |

## 💡 Explanation

Afghanistan and Algeria qualify as big countries because their populations are at least 25 million.

The remaining countries do not meet either the area or population requirement.