# Dex Budget — Guided Beta

A free static progressive web app for testing adaptive budgeting, income modes, bill due dates, and approval-based allocation recommendations.

## Deploy to GitHub Pages
1. Create a GitHub repository (public for free Pages hosting).
2. Upload **the files inside this folder** to the repository root.
3. Go to Settings → Pages → Deploy from branch → main / root → Save.
4. Open the published URL in iPhone Safari and choose Share → Add to Home Screen.

## Important beta limitations
- No bank connections, cloud sync, or payment processing. Data is stored in localStorage on one device; export backups frequently.
- "Safe to spend" is a planning estimate, not a verified bank balance. Reconcile regularly.
- Bills are entered manually and must be updated when paid or rolled to the next due date. A bill payment is an expense and its corresponding bill entry must also be updated; the beta does not automatically link the two.
- The income mode and desired daily savings/fun fields are captured but don't yet implement paycheck forecasting or automatic daily allocation.
- Incoming funds automatically reserve the configured tax percentage, but actual taxes depend on personal circumstances and allowable deductions.
- Expense entries consume fun then essential reserves; they don't yet identify expense categories or automatically apply payments to protected bills. Verify results before relying on them.
- The planning window defaults to 7 days unless a next income date is set. It is not a full long-term cashflow forecast.
- Approval changes are local ledger changes, not bank transfers.
- This is an early prototype. Don't use it as the sole basis for bill payments or financial decisions.

## Test scenarios
1. Add a $800 bill due in 3 days, with $300 protected. Check shortfall and recommendation.
2. Record $200 income. Verify 25% ($50) is reserved for estimated taxes.
3. Record $25 expense. Verify cash decreases exactly once.
4. Approve a flexible-reserve adjustment; check audit and undo.
5. Export backup, clear only after saving, then import and compare totals.
