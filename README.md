# Faillite ou Révolution

A serious game about French public finances, in French. You set the real levers of the budget (VAT, CSG, income tax, retirement age, health spending, public payroll…) from 2026 to 2035. Three judges react: the bond markets, the street, and Brussels. Let the debt run and you end up under IMF supervision. Cut too fast and the government falls.

## Play

Open `index.html` in a browser. It is a single static file with no build step and no dependencies other than Google Fonts.

## How it works

- **Term mode (default).** One budget per year from 2026 to 2035. Random shocks (recession, rate tension, energy crisis, pandemic) are drawn at the start and revealed year by year. Presidential elections in 2027 and 2032, each followed by a snap legislative election.
- **National Assembly.** 577 seats in six blocs (approximate 2024 composition). You pick the governing coalition; none has an absolute majority. Each bloc scores the budget on the anger it causes among its voters by 2030 and, for some, on the deficit avoided, then votes for, abstains, votes against or backs a no-confidence motion. A budget passes with more votes for than against. Otherwise article 49.3 forces it through, unless a censure motion reaches 289 votes. Political capital buys deals with opposition blocs. You can also dissolve the Assembly yourself, at most once a year: the coalition gains seats if anger is below its 2024 level and loses seats above it, give or take 12 seats.
- **Yearly dossiers.** From 2027, most years bring a crisis to settle before the budget vote: farmers' blockades, closing emergency rooms, a steel plant shutting down, a fuel price spike, floods, an EU defence loan, and more (12 in total). Each option costs money, anger, political capital or votes in the Assembly.
- **Turn flow.** A fixed action bar shows where the year stands (dossier, levers, vote) and always carries the next action. Each vote opens a year summary (deficit, debt, rate, anger, capital, and what happened). Results sit in tabs: Assembly, journal, trajectories, who pays, budget, objectives, sources. Under each lever, a chip names the Assembly bloc whose vote that measure moves most. On a phone, levers and results are two screens, switched from the action bar.
- **Tutorial.** A guided tour of eight steps opens on the first visit. The "Comment jouer" button replays it.
- **Sandbox mode.** The same 34 levers held constant from 2026 to 2035, no randomness, everything visible at once.
- **Engine view.** 86 model parameters: end-of-game thresholds, market reaction, anger per group, behavioural responses to taxes, macroeconomics. Every parameter is editable, so a player can test which conclusions depend on which assumption.
- **Model.** Annual loop from 2024 to 2035. Revenue follows actual GDP and spending follows potential GDP. Debt is refinanced at the German rate plus a spread, and the spread reacts with a one-year lag. Social anger follows the losses imposed on each group, with inertia.

## Status

Version 0.9. Figures come from INSEE 2024 accounts (May 2026 revision), PLF, COR, DREES, Unédic, Agence France Trésor and ECB market data as of October 2026. The sourcing work is in `data/sources-2024.md`. Figures without a direct source are flagged as estimates in the game. The anger coefficients are design choices and are flagged as such.

## Credits

Designed by Glamdring Labs.

## License

MIT
