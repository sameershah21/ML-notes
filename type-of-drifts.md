**Notes on "Model Drift in Data Science" Transcript**

---

**1. Introduction:**
- Addressed challenges faced when putting models into production:
    - Need for continuous performance monitoring.
    - Reason for continuous retraining of models.

---

**2. Model Drift:**
- **Definition:** Decline in model performance over time.
- Causes of model drift:
    1. Changes in the relationship between input and output variables.
    2. Overall data distribution alterations.
    3. External factors (e.g., COVID-19 pandemic).
    4. Seasonal changes.
- Main issue: Models trained on past data might not perform well on new, changed data.

---

**3. Types of Model Drift:**
- **Concept Drift:**
    - Related to changes in the properties of the target variable.
    - **Example:** Spam filtering:
        - Initially, emails with the term "lump sum amount" flagged as spam.
        - Scammers adapt, and spam emails become more sophisticated.
        - Result: Model fails to identify new spam patterns.
- **Data Drift:**
    - Deals with changes in the properties of input variables.
    - **Example:** Property Market:
        - Initially, model trained when preference was for 1000 sq. ft. houses.
        - Later, preferences shift to 700-800 sq. ft. apartments due to economic conditions.
        - Result: Model's prediction becomes less accurate.
- **Upstream Changes:**
    - Refers to scenarios where input variables become unavailable or a new variable is added.
    - **Example:** Data pipeline receives null values for an important variable.

---

**4. Detecting Model Drift in Production:**
-  Discuss statistical methods to detect model drift next time.
- Emphasis on identifying drift almost in real-time, not after the availability of ground truth.

---

**5. Conclusion:**
- Understanding different types of drift is crucial.
- Upcoming topic: Methods to identify drift.