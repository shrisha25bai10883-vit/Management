Problem Statement

The core problem this project addresses is the need for a simple, automated system to manage the check-in process and accurately calculate the billing for guests in a small hotel or lodging establishment.

Currently, this process would likely be manual (using paper records or spreadsheets), which is prone to errors in data entry, inconsistency in document verification (Aadhar vs. Passport), and miscalculation of the final amount, especially when accounting for daily rates and taxes like GST.

The solution is a command-line programme that streamlines guest data collection, enforces a basic nationality/document check, and provides an instantaneous, accurate calculation of the total bill including tax.

Scope of the Project
The scope of this project is narrow and focused on two key processes: Guest Data Capture and Basic Billing.

In Scope:

Collecting essential guest information (name, phone, address, nationality, dates).

Implementing a data entry loop to process multiple guests sequentially.

Conditional logic to check for necessary identification (Aadhar/Passport) based on nationality.

Fixed room rate display and selection.

Calculating the total amount based on room rate, days of stay, and a fixed 20% GST rate.

Out of Scope (Current Limitations):

Data Persistence: Data is only stored in memory during the execution (Record dictionary) and is lost when the program closes. It does not connect to a database or save to a file.

Room Inventory Management: The program does not track which rooms are available, occupied, or booked.

Advanced Features: It lacks features like check-out processing, payment integration, employee management, reporting, dynamic pricing, or service/extra charges (e.g., laundry, meals).

User Interface: It is strictly a Command-Line Interface (CLI) application.

Target Users

The primary users of this small-scale application are:

1. Hotel Receptionist/Front Desk Staff: Individuals responsible for the manual process of checking guests into the hotel.

2. Small Hotel Owners/Managers: Those needing a quick, reliable tool to ensure correct billing and basic data capture without investing in complex, expensive software.

High-level features: Guest Check-in and Data Capture, Nationality-Based Document Verification, and Automated Billing and Tax Calculation. 
The system facilitates batch guest check-in by operating within a continuous loop, gathering essential details like name, contact information, address, and stay dates, which are intended to be stored in a record structure.
A key feature is the conditional compliance check, where the system assesses the guest's nationality, prompting specifically for an Aadhar Card number for Indian citizens or generically requiring "Passport Needed" for all other nationalities.
Finally, the program provides core functionality for financial management by allowing the user to select from a menu of four fixed-price room types and then instantly calculating the total cost of stay, which includes the base room rate multiplied by the number of nights, plus a mandatory 20% Goods and Services Tax (GST), outputting both the pre-tax and final amounts.
