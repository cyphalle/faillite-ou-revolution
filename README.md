# Faillite ou Révolution

A serious game about French public finances, in French. You set the real levers of the budget (VAT, CSG, income tax, retirement age, health spending, public payroll…) from 2026 to 2035. Three judges react: the bond markets, the street, and Brussels. Let the debt run and you end up under IMF supervision. Cut too fast and the government falls.

## Play

Open `index.html` in a browser. It is a single static file with no build step and no dependencies other than Google Fonts.

## How it works

- **Term mode (default).** One budget per year from 2026 to 2035. Each measure costs political capital, more so when it hurts. Random shocks (recession, rate tension, energy crisis, pandemic) are drawn at the start and revealed year by year. Presidential elections in 2027 and 2032. When capital runs out, the budget can still pass by article 49.3, at a cost in anger.
- **Sandbox mode.** The same 29 levers held constant from 2026 to 2035, no randomness, everything visible at once.
- **Engine view.** 64 model parameters: end-of-game thresholds, market reaction, anger per group, behavioural responses to taxes, macroeconomics. Every parameter is editable, so a player can test which conclusions depend on which assumption.
- **Model.** Annual loop from 2024 to 2035. Revenue follows actual GDP and spending follows potential GDP. Debt is refinanced at the German rate plus a spread, and the spread reacts with a one-year lag. Social anger follows the losses imposed on each group, with inertia.

## Status

Version 0.4. All figures are 2024 orders of magnitude written from memory. Each one is listed in the in-game sources table with the public source to check (INSEE, PLF, COR, Agence France Trésor, IPP tax tables). They will be replaced by published data before any public release. The anger coefficients are design choices and are flagged as such.

## Credits

Designed by Glamdring Labs.

## License

MIT
