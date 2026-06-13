# Vereins-Webapp Plan

Visuelles Abstimmungsdokument fuer eine Vereins-Webapp mit Google Sheets Backend.

- [PLAN.html](./PLAN.html): visuelle Version mit Mockups
- [PLAN.md](./PLAN.md): textuelle Umsetzungsspezifikation

## Google Workspace

Google Cloud Projekt:

- Project ID: `rider-499313`
- App-Service-Account: `rider-22@rider-499313.iam.gserviceaccount.com`

Drive Root:

- `wsc-prototypes`
- ID: `1DFcRTGyaknZjzLDhbjFK1_IokboR8-4Z`
- URL: https://drive.google.com/drive/folders/1DFcRTGyaknZjzLDhbjFK1_IokboR8-4Z

### Clerk Environment

- Folder `clerk`
  - ID: `1CTGQDIKhe2nKL6HZMQLxfumIsZcjN0IZ`
  - URL: https://drive.google.com/drive/folders/1CTGQDIKhe2nKL6HZMQLxfumIsZcjN0IZ
- Folder `clerk/sessions`
  - ID: `1K1zgFuWrn7dpXwsXfcf25exrsSUE0hRH`
  - URL: https://drive.google.com/drive/folders/1K1zgFuWrn7dpXwsXfcf25exrsSUE0hRH
- Sheet `club_riders`
  - ID: `1Ybr0wRcsbB97J6lqq7pUpX6UXphc6SAXrC_FRcmc9Ys`
  - URL: https://docs.google.com/spreadsheets/d/1Ybr0wRcsbB97J6lqq7pUpX6UXphc6SAXrC_FRcmc9Ys/edit
- Sheet `club_training`
  - ID: `1jE_FiT83l1OTf_Q3jjr3pIT5SwgLfB9yJCvDxlg0rQQ`
  - URL: https://docs.google.com/spreadsheets/d/1jE_FiT83l1OTf_Q3jjr3pIT5SwgLfB9yJCvDxlg0rQQ/edit

### Better Auth Environment

- Folder `better-auth`
  - ID: `1stSLw6JwxDBWfrNv-HKZCTu5ue2u8Aov`
  - URL: https://drive.google.com/drive/folders/1stSLw6JwxDBWfrNv-HKZCTu5ue2u8Aov
- Folder `better-auth/sessions`
  - ID: `1V3iewyflYNF19EZpGgK327MuQWSgff5C`
  - URL: https://drive.google.com/drive/folders/1V3iewyflYNF19EZpGgK327MuQWSgff5C
- Sheet `club_riders`
  - ID: `1rerb0vgAkBi7hStXzvucDDEKUNX7kUYAQpZdlEhPlfo`
  - URL: https://docs.google.com/spreadsheets/d/1rerb0vgAkBi7hStXzvucDDEKUNX7kUYAQpZdlEhPlfo/edit
- Sheet `club_training`
  - ID: `1TfQC6LS963vhooZjtMc_wnes3xtUtiFMzKnEpJY_nJg`
  - URL: https://docs.google.com/spreadsheets/d/1TfQC6LS963vhooZjtMc_wnes3xtUtiFMzKnEpJY_nJg/edit

## Lokale Konfiguration

Die nicht-geheimen Google IDs stehen in [mise.toml](./mise.toml). Secrets wie Service-Account-Private-Keys gehoeren nicht ins Repo.

## Clerk

Clerk-App fuer das Clerk-Environment:

- Name: `WSC Prototypes Clerk`
- App ID: `app_3F5I0r7ipX4ueR77SHBRhBcJTHw`
- Development Instance ID: `ins_3F5I0uuy1tbzHFScNL7pnhahpEr`

Lokale Keys liegen in `.env.local` und werden nicht committed:

- `CLERK_PUBLISHABLE_KEY`
- `NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY`
- `CLERK_SECRET_KEY`

## Better Auth

Better Auth ist selbst gehostet und braucht keine gehostete App-ID.

Nicht-geheime lokale Defaults stehen in [mise.toml](./mise.toml):

- `BETTER_AUTH_URL`
- `BETTER_AUTH_DATABASE_URL`

Lokale Secrets liegen in `.env.local` und werden nicht committed:

- `BETTER_AUTH_SECRET`

1Password Item:

- Vault: `Private`
- Item: `Better Auth - WSC Prototypes`
- Item ID: `ay26htmtpcbltxwxgyo6wecw64`
