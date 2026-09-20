# Privacy Policy

This is a personal, self-hosted integration between [Whoop](https://www.whoop.com) and Claude, built for a single user's own account.

## Data collected

When authorized, this app fetches the following data from the Whoop API on behalf of the authorizing user only:

- Profile and body measurements
- Physiological cycles (strain)
- Recovery scores (HRV, resting heart rate, SpO2, skin temperature)
- Sleep records
- Workout records

## How data is used

Data is cached locally in a SQLite database on the server the user deploys, solely to answer the user's own questions through Claude (e.g. "what's my recovery today?"). It is not shared with any third party, sold, or used for advertising.

## Data storage

OAuth access and refresh tokens are encrypted at rest (AES-256-GCM) before being stored. Health data is stored unencrypted in the same local database, accessible only to the person who deployed and controls the server.

## Data deletion

The user can delete all stored data at any time by deleting the server's database file, or by tearing down the deployment entirely. Revoking app access from the Whoop account settings stops all further data access.

## Contact

This app is maintained by its deployer for personal use. For questions, open an issue on the [source repository](https://github.com/jacksonzuck4-byte/whoop-health).
