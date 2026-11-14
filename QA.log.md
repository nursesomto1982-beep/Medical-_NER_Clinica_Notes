# Quality Assurance & Edge Case Log

| Note ID | Ambiguous Text Extract | Reviewer Note (RN/Clinical Expert) | Resolution & Tag Applied |
| :--- | :--- | :--- | :--- |
| 045 | "Patient is border-line diabetic" | "Border-line" changes the clinical weight of the diagnosis. | Excluded "border-line". Tagged "diabetic" as `CONDITION`. Updated guideline 1.2. |
| 089 | "given sliding scale insulin" | Sliding scale indicates a variable dosage rather than a fixed number. | Tagged "insulin" as `MEDICATION`. Tagged "sliding scale" as `DOSAGE` as it dictates the administration protocol. |
| 112 | "NPO after midnight" | NPO (nil per os) is an instruction, not a medication or condition. | Decided to leave untagged for this specific model iteration. Logged for future `CLINICAL_INSTRUCTION` tag development. |
