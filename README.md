# Scholarship Score Calculation Engine

## Overview

The Scholarship Score Calculation Engine is a robust PL/SQL solution that processes and calculates scholarship scores for teacher applications. This system is designed to automatically compute scores based on several business rules including years of experience, country-based scoring, and extra points for additional working hours. It also includes comprehensive error handling and uses a trigger to generate final results seamlessly.

## Features

- **Modular PL/SQL Implementation:** Separate stored functions for calculating experience score, country score, and extra score.
- **PL/SQL Package:** Contains public constructors and a variable to store the calculated extra score.
- **Error Handling:** Errors during score computation are logged into the `ERROR_PROCESO` table.
- **Automated Result Generation:** A trigger automatically updates the `RESULTADO_POSTULACION` table with the final score and selection status.
- **Dynamic Score Calculation:** Uses input parameters (e.g., the extra score percentage) to compute scores in a flexible manner.

## Project Structure

```plaintext
ScholarshipScoreCalculationEngine/
├── README.md
├── LICENSE
├── .gitignore
├── docs/
│   ├── Evaluation_Instructions.pdf
│   └── Annex_A_Form_A.pdf
└── sql/
   └── ScholarshipScoreCalculation.sql
