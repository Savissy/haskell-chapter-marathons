**Student Eligibility Checker Console App**

📌 Objective
Design and implement a console-based Haskell application that checks whether a student is eligible for a scholarship based on optional inputs.

This project is meant to help you apply core concepts from Chapter 19, especially:

✅ Function application at the Functor level

✅ Purity and effectful computation

✅ The Applicative type class

✅ Applicative laws

✅ Programming with effects (Maybe, IO)

✅ Control.Applicative functions (pure, <*>, liftA2, optional, etc.)

🎯 Task Description
You will build a console app called Student Eligibility Checker that:

Prompts the user (a school administrator) to input student details.

Handles cases where some fields might be missing or skipped.

Uses Maybe as an applicative to apply validation logic.

Outputs whether the student is eligible based on rules below.

✅ Eligibility Rules
A student is eligible if:

GPA is 3.5 or higher

AND participated in extracurricular activities

AND (has financial need OR has a recommendation letter)

Use pure, <*>, and <$> to apply this logic over the Maybe inputs.

🧠 Requirements
Define a Student data type with appropriate fields (Maybe Float, etc.).

Define a function isEligible :: Student -> Maybe Bool that uses Applicative style logic.

Use pure, <*>, <$>, and optionally liftA2, sequenceA, or optional in your implementation.

Use IO to read values from the console.

Skip any field if the user types "skip" or enters nothing.
