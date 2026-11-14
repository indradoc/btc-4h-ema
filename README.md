# btc-cent-forecast-01 entry

Forecasts Bitcoin's price 240 minutes ahead from the pool's 1-minute closes.
Model: 0.7 * last close + 0.3 * slow (12h) EMA — the pool's microstructure
noise decays, so the slow EMA anchors the level; the blend beat the
persistence baseline on all six practice series (1,302 checkpoints, -4.3%).
`main.py` reads $MAKEFUN_INPUT_DIR and writes /output/<id>.out.
License: MIT (SPDX: MIT).
