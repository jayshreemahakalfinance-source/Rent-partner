# Rent Partner — Complete Starter

This is an original professional-companionship marketplace starter.

## Included
Customer website, OTP auth flow, partner registration, partner verification, persistent SQLite database,
bookings, admin dashboard, booking status controls, commission settings, rate limiting, Helmet security headers,
Razorpay order creation adapter, safety rules and production checklist.

## Run
Node.js 18+ recommended.

1. Copy `.env.example` to `.env`.
2. Change `JWT_SECRET` and `ADMIN_PASSWORD`.
3. `npm install`
4. `npm start`
5. Customer: http://localhost:3000
6. Admin: http://localhost:3000/admin/

Demo OTP is `123456` while OTP_MODE=demo.

## Payment
Add Razorpay credentials to `.env` to enable order creation. Never put the secret key in browser code.
For production, implement server-side payment signature verification and webhook reconciliation.

## Production checklist
- Use real OTP provider and SMS templates.
- Use PostgreSQL or managed DB for scale.
- Use HTTPS.
- Store KYC documents in private object storage with encryption and retention rules.
- Add real payment signature verification + webhooks.
- Add CSRF strategy if using cookie auth.
- Add stronger role/permission model and audit logs.
- Add moderation, report/block, dispute/refund workflow.
- Publish Terms, Privacy, Safety, Refund and prohibited-services policies.
- Require applicable age eligibility and identity verification.
- Review Indian legal, tax, consumer-protection, privacy and payment requirements with a qualified professional before launch.
