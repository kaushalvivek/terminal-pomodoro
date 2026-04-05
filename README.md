# pom

A pomodoro timer for your terminal. Seven-segment display, zero dependencies, one file.

```

                          F O C U S

                ━━━    ━━━         ━━━    ━━━
                   ┃  ┃       ●   ┃   ┃  ┃   ┃
                ━━━    ━━━
               ┃          ┃   ●   ┃   ┃  ┃   ┃
                ━━━    ━━━         ━━━    ━━━

               ╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌╌

                          ◐  ○  ○  ○

            space pause · r reset · s skip · q quit

```

## Install

**Homebrew:**

```
brew tap kaushalvivek/pom && brew install pom
```

**Or just download it:**

```sh
curl -fsSL https://raw.githubusercontent.com/kaushalvivek/terminal-pomodoro/main/pom \
  -o /usr/local/bin/pom && chmod +x /usr/local/bin/pom
```

Then run:

```
pom
```

## Controls

| Key | Action |
| --- | --- |
| `space` | pause / resume |
| `r` | reset current timer |
| `s` | skip to next phase |
| `q` | quit |

## The Cycle

```
 ◐ 25m    ○ 5m    ◐ 25m    ○ 5m    ◐ 25m    ○ 5m    ◐ 25m    ◎ 15m
 focus    break   focus    break   focus    break   focus    long break
 ╰──────────────────────── × 4 ────────────────────────╯       then repeat
```

Plays a sound and flashes the screen at each transition.

## Requirements

Python 3 (ships with macOS).

## License

[MIT](LICENSE)
