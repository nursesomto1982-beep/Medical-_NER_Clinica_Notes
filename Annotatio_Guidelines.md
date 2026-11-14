# Annotation Guidelines: Clinical NER v1.0

## Entity Categories

### 1. `CONDITION`
*   **Definition:** Any disease, symptom, diagnosis, or adverse medical event experienced by the patient.
*   **Rule:** Include descriptive adjectives only if they are part of the formal medical diagnosis (e.g., "Type 2 Diabetes"). Do not include severity modifiers like "severe" unless inextricably linked to the clinical term.
*   **Example:** Patient presents with [chronic migraine](CONDITION) and [nausea](CONDITION).

### 2. `MEDICATION`
*   **Definition:** Any pharmacological substance prescribed or taken over-the-counter.
*   **Rule:** Annotate the generic or brand name. Exclude dosages or frequencies from this specific tag.
*   **Example:** Prescribed [Lisinopril](MEDICATION) and [Advil](MEDICATION).

### 3. `DOSAGE`
*   **Definition:** The specific amount or concentration of the medication.
*   **Rule:** Capture the number and the unit of measurement together.
*   **Example:** Take Amoxicillin [500 mg](DOSAGE).

### 4. `FREQUENCY`
*   **Definition:** How often the medication or treatment should be administered.
*   **Rule:** Include clinical abbreviations (e.g., PRN, BID) or plain English equivalents.
*   **Example:** Administer [twice daily](FREQUENCY) or [BID](FREQUENCY).

## Edge Case Handling
*   **Abbreviations vs. Full Text:** Both are tagged identically based on their meaning. "HTN" is tagged as `CONDITION` just like "Hypertension".
*   **Overlapping Entities:** If a condition contains a body part (e.g., "left ventricular hypertrophy"), tag the entire phrase as a single `CONDITION`.
