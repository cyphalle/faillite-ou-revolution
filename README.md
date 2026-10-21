# Faillite ou Révolution

A serious game about French public finances, in French. You set the real levers of the budget (VAT, CSG, income tax, retirement age, health spending, public payroll…) from 2026 to 2035. Three judges react: the bond markets, the street, and Brussels. Let the debt run and you end up under IMF supervision. Cut too fast and the government falls.

## Play

Open `index.html` in a browser. It is a single static file with no build step and no dependencies other than Google Fonts.

## How it works

- **Term mode (default).** One budget per year from 2026 to 2035. Random shocks (recession, rate tension, energy crisis, pandemic) are drawn at the start and revealed year by year. Presidential elections in 2027 and 2032, each followed by a snap legislative election.
- **National Assembly.** 577 seats in six blocs (approximate 2024 composition). You pick the governing coalition; none has an absolute majority. Each bloc scores the budget on the anger it causes among its voters by 2030 and, for some, on the deficit avoided, then votes for, abstains, votes against or backs a no-confidence motion. A budget passes with more votes for than against. Otherwise article 49.3 forces it through, unless a censure motion reaches 289 votes. Political capital buys deals with opposition blocs.
- **Sandbox mode.** The same 34 levers held constant from 2026 to 2035, no randomness, everything visible at once.
- **Engine view.** 84 model parameters: end-of-game thresholds, market reaction, anger per group, behavioural responses to taxes, macroeconomics. Every parameter is editable, so a player can test which conclusions depend on which assumption.
- **Model.** Annual loop from 2024 to 2035. Revenue follows actual GDP and spending follows potential GDP. Debt is refinanced at the German rate plus a spread, and the spread reacts with a one-year lag. Social anger follows the losses imposed on each group, with inertia.

## Status

Version 0.6. Figures come from INSEE 2024 accounts (May 2026 revision), PLF, COR, DREES, Unédic, Agence France Trésor and ECB market data as of October 2026. The sourcing work is in `data/sources-2024.md`. Figures without a direct source are flagged as estimates in the game. The anger coefficients are design choices and are flagged as such.

## Credits

Designed by Glamdring Labs.

## License

MIT
