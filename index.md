# HealthInsights — Privacy Policy

_Last updated: 2026-05-01_

HealthInsights is a personal health-data viewer for individuals managing
type 1 diabetes (or similar conditions) and the family members and care-team
members they choose to share data with.

## What data we collect

- **Apple HealthKit data** you grant access to: blood glucose, insulin
  delivery, heart rate, sleep analysis, exercise minutes, dietary carbs,
  and similar health-and-fitness samples. This data is stored in your
  personal Supabase database (one private database per user) so that
  caregivers you explicitly invite can read it.
- **Account information**: your email address (from Sign in with Apple
  or Google), used solely for sign-in and for inviting caregivers.
- **MCP API access tokens**: opaque tokens generated when you connect a
  third-party MCP-compliant client (e.g., Claude.ai). Stored hashed in
  your Supabase database. Revocable from Settings.

## What we do NOT collect

- We do not use third-party analytics, ad SDKs, or telemetry services.
- We do not sell, rent, or share your data with anyone you have not
  explicitly granted access to.
- We do not retain any data on devices other than your own iPhone, your
  Supabase database, and (if granted access) your invited caregivers'
  iPhones.

## Where data lives

- Your iPhone (HealthKit, encrypted at rest by iOS).
- A Supabase Postgres database scoped to your user account, accessible
  only to you and caregivers you've invited (enforced by row-level
  security).
- A small subset of weekly aggregate insights is sent to Anthropic
  (Claude API) once a week to generate a digest narrative emailed to your
  invited caregivers. Per Anthropic's API terms, these requests are not
  used to train models.

## Your rights

- You can revoke any caregiver's access from the iOS app at any time.
- You can revoke any connected MCP client's access from Settings →
  Connected apps.
- You can request deletion of your Supabase data by emailing
  carl.christian.christensen@gmail.com.

## Children

This app is intended for adults managing their own data, or for adult
parents/guardians managing data for minor children with chronic conditions.
We do not knowingly collect data directly from children under 13 except
through a parent's HealthKit account.

## Contact

Carl Christian Christensen — carl.christian.christensen@gmail.com
