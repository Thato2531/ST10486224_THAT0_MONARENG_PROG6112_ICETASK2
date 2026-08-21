# ST10486224_THAT0_MONARENG_PROG6112_ICETASK2
# ICE TASK 2: Clinic Patient Management System

## Project Description

The Clinic Patient Management System is a console-based Java application developed to help a small community health clinic manage patient records, appointments, doctor schedules, and clinic reports.

The system replaces the manual paper-based process with a simple computerised system. It allows clinic staff to register patients, manage patient information, schedule and cancel appointments, and generate basic reports.

The application is designed for a clinic with 15 appointment slots arranged across three days: Monday, Tuesday, and Wednesday.

---

## Features

### Patient Management

The system allows users to:

- Register a new patient
- Search for a patient using their Patient ID
- Update patient details
- Delete a patient
- Display all registered patients
- Prevent duplicate Patient IDs

Each patient stores the following information:

- Patient ID
- First Name
- Last Name
- Date of Birth
- Contact Number
- Email Address
- Medical History
- Patient Type

---

## Patient Categories

The system supports three patient categories:

### General Patient

General patients can schedule appointments online.

Additional information stored for a General Patient:

- Preferred Doctor
- Insurance Provider

The `GeneralPatient` class extends the `Patient` class and demonstrates inheritance and method overriding.

### Specialist Patient

Specialist patients use the base `Patient` class and require specialist consultation.

### Chronic Patient

Chronic patients use the base `Patient` class and require regular check-ups.

---

## Appointment Management

The clinic contains 15 appointment slots.

### Appointment Schedule

| Day | Available Times |
|-----|-----------------|
| Monday | 9:00 AM, 10:00 AM, 11:00 AM, 2:00 PM, 3:00 PM |
| Tuesday | 9:00 AM, 10:00 AM, 11:00 AM, 2:00 PM, 3:00 PM |
| Wednesday | 9:00 AM, 10:00 AM, 11:00 AM, 2:00 PM, 3:00 PM |

The system allows users to:

- Schedule an appointment
- Cancel an appointment
- View the complete clinic schedule
- View available appointments
- View booked appointments
- Prevent double-booking
- Prevent a patient from having more than one appointment

Only General patients can schedule appointments.

---

## Reports

The system can generate the following reports:

- All registered patients
- All available appointments
- All booked appointments
- Total number of registered patients
- Total number of booked appointments
- Clinic occupancy percentage

The clinic occupancy percentage is calculated using:

```text
(Number of Booked Appointments / Total Appointment Slots) × 100
