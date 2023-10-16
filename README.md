# Top 3 Section SQL Interview

1. Normalisation
   Normalisation is a database design technique to remove or avoid redundancy in the data. Data Redundancy is nothing but data duplication in records.

2. How to implement normalisation?

   1. 1NF
      - Every column should have a single value.
      - Each row should be unique, either through a single or multiple columns. It's not mandatory to have a primary key.

   2. 2NF
      - Must be in 1NF.
      - All non-key attributes must be fully dependent on the candidate key.
        (Non-key attributes are elements that are not part of the primary key in the table.)
        - Candidate key is created by concatenating two or more columns to make the data unique.

   3. Every table should have a primary key, and relationships between tables should be formed using foreign keys.

3. 3NF
   1. Must be in 2NF.
   2. Avoid transitive dependencies.
      - Transitive Dependencies: If you have a table T with three columns, namely A, B, and C, and A is functionally dependent on B, and B is functionally dependent on C, then we can say that A is functionally dependent on C.

## Different Anomalies
- Insertion : Adding records in Denormalized table, say 4 example on e of your customer was buying 2 type of product and after 4 years he started buying 8 types of profuct then we insert records for newly product.
- Deletion: Removing item whihc is not required.
- Updation: updation cause of change for same item.

Please write in English language.
