# Smart Expense Tracker using Google Apps Script
This project is an automated expense tracking system built on Google Workspace tools and APIs. It reads Gmail receipts, extracts and categorizes data, pushes them to Google Sheets, and visualizes your spending. It also provides real-time SMS alerts using Twilio and maintains a fault-tolerant logging system.

## Features

- Automatically fetches emails from a specific Gmail label (`Expense_Receipts`)
- Extracts structured data from email subject lines and content
- Downloads attachments (like invoices) and saves them to Google Drive
- Populates and categorizes entries into a Google Sheet
- Generates real-time spending graphs in Google Sheets
- Sends SMS alerts for new or critical expenses using Twilio API
- Maintains logs for processed/unprocessed mails and error handling
- Retries failed attempts for improved fault tolerance

## Tech Stack

- Google Apps Script (Gmail, Drive, Sheets APIs)
- Twilio API (for SMS notifications)
- Google Sheets (Data visualization)
- Gmail filters and labels

## How to Deploy

1. Copy this repo to your [Google Apps Script](https://script.google.com/) environment.
2. Set your Gmail filter to label receipts as `Expense_Receipts`.
3. Create a Google Sheet using the included template.
4. Set up a Twilio account and insert credentials in `Twilio.gs`.
5. Run `setupTriggers()` to enable automation.

