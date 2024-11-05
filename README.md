# Introduction
The E-Voting in Homomorphic Encryption in Cloud project is an innovative web development application that enhances the security and privacy of electoral processes through advanced cryptography. This online voting system ensures voter confidentiality by using homomorphic encryption to enable votes to be cast and counted without disclosing individual choices.  The project utilizes a cloud-based MongoDB database to securely store user credentials and encrypted votes, enabling efficient management by administrators. This project intends to offer a strong and user-friendly platform for holding elections while preserving the secrecy and integrity of the voting process, with separate user roles for administrators, candidates, and voters.

When a vote is cast, it is added to the candidate's existing encrypted vote count in real-time. The administrator's sole responsibility is to decrypt the final tally using their private key, ensuring the confidentiality of individual votes. This real-time vote aggregation distinguishes this project from others in the field.

## Table of Contents

1. [Features](#features)
2. [Technologies Used](#technologies-used)
3. [Installation & Setup](#installation--setup)
4. [Usage Guide](#usage-guide)
5. [Security Considerations](#security-considerations)
6. [License](#license)

## Features

- **Secure Voting Process**: Utilizes homomorphic encryption to maintain voter confidentiality while allowing votes to be counted without revealing individual choices.
- **Real-Time Vote Aggregation**: Votes are added in real-time to the candidate's existing encrypted vote count, ensuring up-to-date results.
- **Role-Based Access Control**: Differentiates user roles for administrators, candidates, and voters, enhancing security and user management.
- **Cloud-Based Database**: Employs MongoDB for secure storage of user credentials and encrypted votes, providing reliable data management.

- ## Technologies Used

- **Programming Languages**: Python, JavaScript
- **Frameworks**: Flask for web development
- **Database**: MongoDB for cloud-based data storage
- **Cryptography**: Paillier homomorphic encryption for secure voting

## Installation & Setup

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/shashankrxj/E-Voting-with-Homomorphic-Encryption.git

2. Navigate to the project directory:
   ```bash
   cd E-Voting-Homomorphic-Encryption-Cloud

3. Set up your MONGO_URI and SECRET_KEY
   ```bash
   MONGO_URI = Your MONGO_URI in db.py file for having database connection
   SECRET_KEY = Your SECRET_KEY in app.py for having session management

5. Install the required packages:
   ```bash
   pip install -r requirements.txt

## Usage Guide

1. Register Users:
   Use the registration routes to create administrator, candidate, and voter accounts.

2. Casting Votes:
   Voters log in, select their candidate, and cast an encrypted vote.

3. Tallying Votes:
   Administrators can calculate the election results by decrypting the vote totals and viewing the results.

4. Resetting the Election:
   Use the reset button to clear votes and reset the database for a new election.

## Role






