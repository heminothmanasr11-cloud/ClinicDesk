# ClinicDesk Sync — Firebase

## Included
- index.html: the synchronized ClinicDesk app
- firestore.rules: role-based Firestore access rules
- firebase.json: Firebase Hosting configuration

## Before opening the app
1. Firebase Console → Authentication → Sign-in method → enable Email/Password.
2. Firebase Console → Firestore Database → Create database.
3. Publish the included Firestore rules.

## First setup
Create the Doctor account first, then create the Secretary account.

## Hosting
From a computer with Firebase CLI:
firebase login
firebase use clinic-system-1959d
firebase deploy

The same hosted ClinicDesk URL can then be opened on both laptops.

## Important security note
This is a functional prototype. Because the first account role is selected during registration, production use should move role assignment to a trusted administrator process using custom claims or a server-side function. Do not use real patient data until security, privacy, backups, and applicable healthcare/data-protection requirements have been reviewed.
