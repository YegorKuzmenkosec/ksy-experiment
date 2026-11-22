# KSY — Fact Integration Experiment

A bilingual (Russian/Czech) cognitive-systems pilot study investigating how the number and placement of relevant facts affect question-answering accuracy and response time in humans and language models.

## Human experiment

- [Language selection](https://yegorkuzmenkosec.github.io/ksy-experiment/)
- [Russian](https://yegorkuzmenkosec.github.io/ksy-experiment/ru.html)
- [Czech](https://yegorkuzmenkosec.github.io/ksy-experiment/cz.html)

The participant completes six trials (two each at levels A/B/C). The design includes **grouped** and **distributed** placement of relevant information. After finishing, the participant downloads a CSV file and sends it to the researcher. **GitHub Pages does not collect or store responses automatically.**

## Data format

Each trial CSV includes: `session`, `trial`, `scenario`, `level`, `condition`, `required_facts`, `answer`, `correct_answer`, `correct`, `response_ms`.

Keep Russian and Czech results separate in analysis: language is an experimental variable. Do not publish participant-identifiable information. Preserve original CSV files.

## Current status

- [x] Bilingual participant-facing HTML
- [x] Client-side trial randomization and CSV export
- [ ] Collect and verify participant CSVs
- [ ] Reproducible LLM evaluation on matching stimuli
- [ ] Statistical analysis and plots
- [ ] Final report

## Research integrity

Only measured observations belong in the empirical results. Simulated data, if used for software testing or illustration, must be clearly labeled as synthetic and excluded from empirical conclusions. With small samples, report descriptive statistics and uncertainty; do not claim population-level findings.

## Next steps

1. Gather the actual CSV exports from participants.
2. Confirm the exact assignment requirements and the LLM model/runtime.
3. Run LLM evaluations with saved raw outputs and deterministic settings.
4. Analyze by language, number of facts, and grouped/distributed condition.
5. Prepare a reproducible report with limitations.
