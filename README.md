# Smart Factory Stochastic Simulator — Presentation Version

Streamlit dashboard for a multi-product stochastic discrete-event smart-factory simulation.

## Presentation upgrades
- Animated 10-second replay of the complete simulated factory history.
- Compact branch/merge factory schematic with live product tokens, queues and machine states.
- Manual replay slider retained for inspection.
- "Highest-utilization station" wording instead of claiming a universal bottleneck definition.
- Validation checks moved into technical details.
- Event log collapsed into a technical expander.
- Parameter table explicitly distinguishes workbook-derived values from synthetic engineering assumptions.

## Run locally
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Model basis
Product routing and the known 25 s (MC6/MC7) and 5 s (MC8/MC9) processing times are derived from the supplied workbook. Missing cycle-time, variability, reliability and repair parameters are synthetic assumptions for demonstration and can later be replaced without changing the event logic.
