# Faillite ou Révolution

A serious game about French public finances, in French. You set the real levers of the budget (VAT, CSG, income tax, retirement age, health spending, public payroll…) from 2026 to 2035. Three judges react: the bond markets, the street, and Brussels. Let the debt run and you end up under IMF supervision. Cut too fast and the government falls.

## Play

Open `index.html` in a browser. It is a single static file with no build step and no dependencies other than Google Fonts.

## How it works

- **Term mode (default).** One budget per year from 2026 to 2035. Random shocks (recession, rate tension, energy crisis, pandemic) are drawn at the start and revealed year by year. Presidential elections in 2027 and 2032, each followed by a snap legislative election.
- **National Assembly.** 577 seats in six blocs (approximate 2024 composition). You pick the governing coalition; none has an absolute majority. Each bloc scores the budget on the anger it causes among its voters by 2030 and, for some, on the deficit avoided, then votes for, abstains, votes against or backs a no-confidence motion. A budget passes with more votes for than against. Otherwise article 49.3 forces it through, unless a censure motion reaches 289 votes. Political capital buys deals with opposition blocs. You can also dissolve the Assembly yourself, at most once a year: the coalition gains seats if anger is below its 2024 level and loses seats above it, give or take 12 seats.
- **Yearly dossiers.** From 2027, most years bring a crisis to settle before the budget vote: farmers' blockades, closing emergency rooms, a steel plant shutting down, a fuel price spike, floods, an EU defence loan, and more (12 in total). Each option costs money, anger, political capital or votes in the Assembly.
- **Turn flow.** A fixed action bar shows where the year stands (dossier, levers, vote) and always carries the next action. Each vote opens a year summary (deficit, debt, rate, anger, capital, and what happened). Results sit in tabs: Assembly, journal, trajectories, who pays, budget, objectives, past games, sources. Under each lever, a chip names the Assembly bloc whose vote that measure moves most. On a phone, levers and results are two screens, switched from the action bar.
- **Live forecast.** During a year, the dashboard shows what the budget being drafted would give for the deficit (Brussels), the 10-year rate (markets) and anger (the street), so every lever step moves it. The year's random shocks stay hidden until the vote, and the year summary shows forecast against outcome.
- **Simpler levers.** The twelve heaviest levers show first; the others unfold and stay visible once changed. Each range lever has − and + buttons that move one readable step.
- **Tone.** Each vote ends with the next morning's front page from an imaginary newspaper, levers pushed to the end of their range get a one-line quip, and every ending has a title ("Le syndrome d'Athènes", "Le Pinay du XXIe siècle", "Après moi, le déluge"). The jokes target institutions and habits of every camp, never a person.
- **End-of-term summary.** Win or lose, the game closes on a summary: one tile per budget (voted, 49.3, fatal year), debt and deficit from start to end, interest paid in aircraft carriers, debt added in baguettes per person, peak anger, 49.3 count, credit rating, angriest group, time in office against the Fifth Republic average, and the whole press review.
- **Difficulty.** Three levels, picked before the first vote or for the next game: Facile (fewer shocks, more capital, more patient street and markets), Difficile (the default calibration) and Dinguerie (a shock almost every year, a dossier every year, nervous markets, an angrier street and a trigger-happy Assembly). Each level only sets engine parameters, so every value stays visible in the engine view.
- **Verdict.** Every game ends on one of the title's two words, or on a win. Bankruptcy ("Faillite") is the IMF taking over once the 10-year rate crosses its threshold. Revolution ("Révolution") is the government brought down by the street, by a censure motion, or by losing the presidential election. The summary says which judge gave up first, and shows how close the game came to each outcome (peak rate against the IMF threshold, peak anger or censure votes against theirs).
- **History.** Each finished game is saved in the browser: date, difficulty, coalition, number of turns played, outcome (bankruptcy, revolution or win), and final deficit, debt and anger. The last five show in the end-of-term summary, and all of them in the "Parties" tab.
- **Replay.** A lost game says by how much it was lost (votes short, points over the threshold) and can be replayed with the same seed: same shocks, same dossiers, same years.
- **Tutorial.** A guided tour of eight steps opens on the first visit. The "Comment jouer" button replays it.
- **Sandbox mode.** The same 34 levers held constant from 2026 to 2035, no randomness, everything visible at once.
- **Engine view.** 86 model parameters: end-of-game thresholds, market reaction, anger per group, behavioural responses to taxes, macroeconomics. Every parameter is editable, so a player can test which conclusions depend on which assumption.
- **Model.** Annual loop from 2024 to 2035. Revenue follows actual GDP and spending follows potential GDP. Debt is refinanced at the German rate plus a spread, and the spread reacts with a one-year lag. Social anger follows the losses imposed on each group, with inertia.

## Status

Version 0.14. Figures come from INSEE 2024 accounts (May 2026 revision), PLF, COR, DREES, Unédic, Agence France Trésor and ECB market data as of October 2026. The sourcing work is in `data/sources-2024.md`. Figures without a direct source are flagged as estimates in the game. The anger coefficients are design choices and are flagged as such.

## Credits

Designed by Glamdring Labs.

## License

MIT
