Here's a high-level explanation of the output you can expect when running the provided script. This script is for managing a hospital's health diagnosis system using SQLite and involves various functionalities:

Database Initialization:

When the script runs, it first checks if the necessary tables (doctor, patient, virus, bacteria, injury) exist in the hospital.db SQLite database.
If any of these tables do not exist, the script creates them with the specified schema.
Main Menu:

After ensuring the database is set up, it presents a main menu for logging in or creating a new account.
Account Creation:

If you choose to create a new account (e=2), you will be prompted to enter details for a new doctor, including their ID, name, password, specialty, shift, and phone number. This information is then inserted into the doctor table.
Log In:

If you choose to log in (e=1), you will need to provide a doctor ID and password.
If the ID and password are correct, you will see a successful sign-in message and be taken to a menu where you can:
View patient details.
Add a new patient.
Delete patient details.
Viewing Patient Details:

You can enter a patient ID to view details. If the patient exists, you will see their basic information and any associated records of virus, bacteria, or injury. If the patient doesn't exist, you will see an error message.
Adding a New Patient:

You will be prompted to enter details for a new patient, including their ID, name, city, DOB, age, date of admission, and phone number.
After adding a patient, you can also input related medical information (virus, bacteria, or injury).
Deleting Patient Details:

You can delete a patient’s records by entering their ID. If the patient exists, their details and any associated records in virus, bacteria, and injury tables will be deleted.
Viewing All Records:

If you enter 2212, the script will display all records from the doctor, virus, bacteria, and injury tables.
Backup:

Finally, the script attempts to create a backup of the hospital.db database into hospital_backup.db. It prints a success message if the backup is successful or an error message if it fails.
