Here’s a detailed but concise comparison of **SQL** versus **true relational theory** as proposed by Edgar F. Codd:

| Aspect                     | SQL                                                                                     | True Relational Theory (Codd)                                                                      |
| -------------------------- | --------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **Foundation**             | Based on relational concepts but includes deviations for practical purposes.            | Strictly based on Codd’s 12 rules defining a relational database.                                  |
| **Data Representation**    | Tables (relations) but allows duplicates and NULLs.                                     | Relations are sets of tuples; no duplicates allowed, and NULLs are not part of the original model. |
| **Keys**                   | Primary keys supported; foreign keys optional; sometimes not strictly enforced.         | Every relation has a candidate key; all relationships are expressed via keys.                      |
| **Normalization**          | Normalization is possible but often partial; denormalization is common for performance. | Full normalization is a core requirement; redundancy is minimized.                                 |
| **Integrity Constraints**  | Referential integrity and constraints are enforced but may vary by implementation.      | Integrity rules are mandatory; every tuple must satisfy the relational constraints.                |
| **Operations**             | SQL provides SELECT, INSERT, UPDATE, DELETE, JOIN, etc.                                 | Relational algebra and relational calculus define formal operations (strict mathematical model).   |
| **NULLs**                  | Supported; represent missing or unknown information.                                    | Not allowed; “unknown” values violate the strict set theory model.                                 |
| **Practicality vs Theory** | Prioritizes ease of use, performance, and backward compatibility.                       | Prioritizes mathematical purity and consistency.                                                   |
| **Example Issues**         | In SQL, a table can have duplicate rows, violating the uniqueness of tuples.            | In true relational theory, duplicates are forbidden; every tuple is unique by definition.          |

**Summary:**
SQL is inspired by relational theory but sacrifices some theoretical purity for practical usability (e.g., NULLs, duplicates, optional constraints). True relational theory is mathematically rigorous and avoids ambiguities, but implementing it fully in a real-world system is rare.

---

