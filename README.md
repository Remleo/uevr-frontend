# UEVR.Frontend

The frontend injector for the UEVR mod. Does not contain the actual mod itself.

## Auto-inject

This fork adds auto-inject: a game is injected as soon as it is running, with no need to pick the process and
press Inject. It is switched on per game, in that game's `config.txt`:

```
Frontend_AutoInject=true
Frontend_AutoInjectDelay=5
```

- `Frontend_AutoInject` — inject this game automatically. Off by default.
- `Frontend_AutoInjectDelay` — seconds to wait after the game is ready, for games that crash when injected too
  early. `0` injects at once.
