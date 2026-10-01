SAMIA'S CLOSET V10

What changed:
- Admin panel is gated by Google account email rahihumaun369@gmail.com.
- The admin app stays hidden until Firebase Auth confirms the exact owner account.
- Orders, visitors, reward users, vouchers, quiz attempts, mystery boxes and quiz questions are visible in Admin.
- Product, combo, website, story and contact settings remain editable.
- Customer rewards now use Firebase Auth + Firestore records instead of only localStorage.
- Daily quiz is limited to one attempt per authenticated visitor per day.
- A quiz question is recorded in lifetime history for that visitor and cannot be used again through the Firestore rules.
- Mystery box is limited to one record per authenticated visitor per week.
- Voucher usage is stored in Firestore.
- Orders store the authenticated visitor ID when available.

IMPORTANT:
1) Deploy this whole folder/ZIP to the same Netlify site.
2) Publish firestore.rules from this package in Firebase Console -> Firestore Database -> Rules.
3) The owner Google account must be rahihumaun369@gmail.com and email verified.
4) Firebase Auth must have Google provider and Anonymous sign-in enabled.

SECURITY NOTE:
A static web app cannot guarantee a physical "one phone only" limit against a determined user who clears app data or uses another browser/device identity. This build enforces one per Firebase-authenticated visitor. A truly device/phone-bound guarantee requires phone verification or a trusted backend (e.g. Cloud Functions) for reward issuance.
