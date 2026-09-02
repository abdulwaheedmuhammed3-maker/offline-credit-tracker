# KioskLedger: Offline-First Micro-Credit & Float Tracker

## The User
Informal POS kiosk operators and market traders in high-density commercial centers across Ilorin (such as Ipata Market and Tanke) who handle micro-transactions and manual credit logs.

## The Problem
Network instability and sudden downtime paralyze digital agency banking and credit tracking, forcing traders to rely on loose paper slips that are easily lost, damaged by weather, or disputed.

## What Was Built
A client-side Vanilla HTML/JS/CSS single-file app utilizing browser LocalStorage to record, timestamp, and display localized micro-credit and float entries completely offline without external server dependencies or internet connectivity.

## Known Limitations
- Data storage is restricted to the local browser instance; if browser cache is entirely cleared without a peer-to-peer sync backup, local records will be wiped.
- The prototype does not include automated SMS cellular fallback or multi-device mesh Bluetooth syncing in this barebones phase.

## Verification Checks
1. **Offline Execution Check:** Turn off your Wi-Fi/cellular data completely, load the HTML file in your browser, enter a transaction (e.g., "Mama Rukayat", 5000), and confirm it renders instantly.
2. **Persistence Check:** Refresh the browser page or completely close and reopen the file; verify that the previously entered transaction remains saved via LocalStorage.
3. **Validation Guard Check:** Attempt to submit the form with empty input fields; confirm that the validation error alert triggers successfully without executing a blank log entry.
