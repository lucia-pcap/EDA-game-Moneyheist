#  EDA game: Money Heist 25-26 Q1

Programming tournament of the EDA (Data Structures and Algorithms) course at FIB-UPC.

🏆 My player **Yuta5** (in `/joc/MY_PLAYERS/`) survived **294 of 302** elimination rounds, finishing in the **top 8**.

## Usage

### Requirements

- `g++` with C++11 support or later
- `make`
- A modern web browser (Firefox, Chrome or Safari) for the viewer

> **Note:** The game engine, HTML viewer and `default.cnf` were provided by the EDA course staff and are not included in this repository.

### Build

From the game directory, select the precompiled object for your architecture and compile:

```bash
cd joc
cp AIDummy.o.Linux64 AIDummy.o
make all
```

### Run a match

```bash
./Game Yuta5 Demo Demo Demo -s 30 < default.cnf > game.res
```

| Argument | Description |
|---|---|
| `Yuta5 Demo Demo Demo` | The four players in the match |
| `-s 30` | Random seed (use different seeds to test different games) |
| `< default.cnf` | Board and game configuration |
| `> game.res` | Output file with the full match record |

Run `./Game --list` to see all available players, or `./Game --help` for more options.

### Watch the match

Open `viewer.html` in your browser and load `game.res`..
