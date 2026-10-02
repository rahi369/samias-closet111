# SAMIA'S CLOSET — Firebase starter

## 1. Install
npm install

## 2. Run
npm run dev

## 3. Firebase
Project: samia-s-closet-new-8f9d0
Auth: Email/Password + Google
Firestore + Storage should be enabled in Firebase Console.

## 4. Deploy rules
Install Firebase CLI, login, then:
firebase use samia-s-closet-new-8f9d0
firebase deploy --only firestore:rules,firestore:indexes,storage

## 5. Important
This package includes the supplied Firebase Web config, rules, storage rules, and a clean UI/core Firebase connection. It is NOT claimed as fully production-tested. Checkout/order callable backend, complete admin CRUD, quiz/voucher atomic enforcement, mystery-box allocation, streak/gift automation and end-to-end security testing still require implementation/testing before production.
