# Privacy Policy — oura-morning

_Last updated: 2026-09-28_

oura-morning is a personal, non-commercial project that reads data from a user's own Oura account to produce a daily recovery summary. This page explains what it accesses, where the data goes, and how to remove it.

## What data is accessed
With the user's explicit OAuth authorization, the app reads (only the scopes the user approves): personal info, daily sleep / readiness / activity / stress summaries, sleep sessions (including heart rate and HRV), workouts, heart rate, SpO₂ and user-created tags.

## Where the data is stored
- **Locally only.** Tokens and fetched data are stored as files on the user's own computer (`~/.oura/`) or, if the user chooses to run it on GitHub Actions, in that user's own **private** repository.
- The developer has no server that receives, stores, or has access to your Oura data.
- No analytics, advertising, or tracking is used. Data is never sold or shared.

## Optional third parties (off by default; user-configured)
- **Push notifications:** if you configure a push channel (e.g. ntfy, Bark, Server酱, Telegram), a short summary message is sent to that service.
- **LLM polishing:** if you configure an LLM endpoint, a summary of your daily metrics (no name or contact details) is sent to the provider you chose, at most once per day.
These services have their own privacy policies; you control whether they are used.

## Your control
- **Revoke access** at any time from your Oura account's connected-applications settings.
- **Delete data** by deleting the `~/.oura/` folder (or the private repository / its `state` branch).

## Changes
If the project later offers a hosted service, this policy will be updated **before** it collects any data from other people, and hosting will be opt-in.


_This page is a plain-language description of the project's behavior, not legal advice._
