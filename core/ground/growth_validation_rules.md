# Growth grounding and validation rules

This file specifies the minimal validation contract for the **Growth Without Profit** technical proof. It is not a production evaluation pipeline.

## Proposed deterministic checks

1. Every claim must reference at least one existing evidence ID.
2. `E1` contains the supporting unit-economics calculation: contribution margin is `(revenue - discount - shipping - CAC - product cost) / revenue`, represented in the prototype as 18.2% baseline and 3.1% current.
3. Evidence references must use the fixture IDs `E1` and `E2`; a future validator would reject unknown IDs.
4. The proposed intervention may be `raise_free_shipping_threshold`, but the numerical threshold is human-owned. The demo decision remains **$50 → $65**.
5. Guardrails remain contribution profit `> +5%`, revenue impact `> -3%`, and conversion impact `> -5%`.

## Evidence sufficiency behavior

- With `E1` and `E2`, the output may state the near-term economic claim and must retain the long-term-value qualification.
- With `E1` only, the output must mark missing customer-value context; it must not label the campaign ineffective.
- Without a valid supporting evidence reference, the output must request the missing metric or source record instead of making a business conclusion.

## Responsibility boundary

The browser prototype implements the displayed calculations and source trace. The AI interpretation, option generation, and contextual retrieval are simulated structured behavior. A future live implementation would validate model output against these rules before presentation.
