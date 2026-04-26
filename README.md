# Wealth Tracker

A free-to-use desktop application for tracking and analyzing your personal wealth across multiple accounts and currencies.

## Features

- **Multi-Account Tracking:** Cash, Equity, Mutual Funds, NPS, PPF, EPF, PRS, Fixed Deposits, Credit Cards, Loans
- **Multi-Currency Support:** Track accounts in different currencies with live conversion rates
- **Transaction Recording:** Income, expenses, transfers, investments, redemptions, and more
- **Mark-to-Market Valuation:** Update asset prices to reflect current market values
- **Comprehensive Reports:** View total wealth snapshot and detailed transaction history
- **Secure Backup & Restore:** Encrypted database backups with AES-256-GCM encryption
- **First-Run Guided Tour:** Interactive onboarding to help new users get started
- **Local-First Privacy:** All data stays on your machine; no cloud, no telemetry

## Installation

### macOS

**Via Homebrew (coming soon):**
```bash
brew install shaileshjoshi/wealth-tracker/wealth-tracker
```

**Direct Download:**
1. Download the latest `.dmg` installer from [Releases](https://github.com/shaileshjoshi/wealth-tracker/releases)
2. Open the `.dmg` file
3. Drag "Wealth Tracker" to Applications
4. Open Wealth Tracker from Applications folder

### Windows (Post-v1)

Windows support is planned for a future release.

## Quick Start

1. **Launch the app** and follow the guided tour (or click "Take Tour" in the top-right anytime)
2. **Set your base currency first** (Settings → Currency): 
   - Select your base currency (e.g., INR, USD)
   - Click "Save" and confirm in the popup (base currency cannot be changed later)
   - All wealth will be tracked in this currency
3. **Create accounts** (Settings → Accounts): Add cash, equity, mutual funds, credit cards, loans, etc. (only available after base currency is set)
4. **Record transactions** (Orders): Income, expenses, transfers, investments
5. **Set currency rates** (Settings → Currency): For multi-currency conversions
6. **Update prices** (Settings → Price): Asset prices for equity, mutual funds, NPS, PRS
7. **View reports** (Reports): Total wealth snapshot and detailed transaction history
8. **Check Dashboard:** View your entire wealth at a glance

## Guided Tour

Click the **"Take Tour"** button in the top-right corner to walk through the onboarding tour at any time. The tour covers:
1. Base currency setup
2. Account creation
3. Transaction tracking
4. Currency rates
5. Asset pricing
6. Reports
7. Dashboard overview

## Backup & Recovery

### Create a Backup

1. Go to **Settings → Database**
2. Click **"Create Backup"** (optionally add a password for encryption)
3. Backup file is saved to your application directory with a timestamp

### Restore from Backup

1. Go to **Settings → Database**
2. Click **"Restore Backup"**
3. Select a backup file (enter password if encrypted)
4. **Restart the app** after restore completes

### Manual Database Copy

Your database file is located at the path shown in Settings → Database. You can manually copy this file as a backup to any location for long-term storage.

## Supported Account Types

- **Cash:** Checking, savings, or other cash accounts
- **Equity:** Stock investments
- **Mutual Fund:** Mutual fund holdings
- **NPS:** National Pension System (India)
- **PPF:** Public Provident Fund (India)
- **EPF:** Employee Provident Fund (India)
- **PRS:** Pension Retirement Scheme (India)
- **Fixed Deposit:** Time-bound fixed-rate deposits
- **Credit Card:** Credit card accounts
- **Loan:** Loan accounts (mortgages, personal loans, etc.)

## Troubleshooting

### App won't start
- Try restarting your computer
- Ensure you have the latest macOS updates installed
- Check that you have write permissions to your home directory

### Can't restore from backup
- Verify the backup file is not corrupted
- If the backup was encrypted, ensure you enter the correct password
- Try copying the database file manually (see Backup & Recovery section)

### Transactions aren't showing
- Refresh the Reports page
- Check that the correct account is selected in account filters
- Verify the date range includes your transactions

### Balance mismatch
- Run a manual recalculation (this happens automatically, but can be verified in database)
- Check for duplicate transactions or transfers
- Create a backup and try restoring to a known good state

## Privacy & Security

**Your data stays local.** All financial information is stored on your machine in an encrypted SQLite database. No data is sent to external servers. See [PRIVACY.md](PRIVACY.md) for full details.

- **Zero telemetry:** No analytics, crash reports, or usage tracking
- **Encrypted backups:** AES-256-GCM encryption for backup files
- **Local-only:** Completely offline operation
- **Source code rights reserved:** Source reuse, modification, or redistribution requires explicit written consent from the author

## Roadmap & Future Features

### v1.0.0 (Current)
- ✅ Multi-account tracking
- ✅ Multi-currency support
- ✅ Comprehensive reports
- ✅ Backup/restore
- ✅ Guided onboarding tour

### Planned (Future - Free Tier Unchanged)
- [ ] Advanced analytics and insights
- [ ] Multi-device synchronization (optional, encrypted)
- [ ] Mobile app companion (optional)
- [ ] Advisor collaboration tools (optional)
- [ ] Additional export formats (JSON, Excel)
- [ ] Windows and Linux support

**All future features will remain optional and will not reduce free-tier functionality.**

## Support

- **GitHub Issues:** Report bugs or request features on [GitHub](https://github.com/shaileshjoshi/wealth-tracker/issues)
- **Documentation:** Refer to this README, PRIVACY.md, and the in-app guided tour

## License

Wealth Tracker is free to use. The source code remains proprietary intellectual property of the author. See LICENSE for usage terms.

## Contributing

Community contributions are welcome. Please see CONTRIBUTING.md (coming soon) for guidelines.

---

**Version:** 1.0.0  
**Last Updated:** 26 April 2026
