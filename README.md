# Money

> But if you ask for a rise<br/>
> It’s no surprise that they’re giving none away
>
> — Pink Floyd, _Money_

A personal finance manager. Work in progress.

Loads transaction data from banking export CSVs, normalizes the data, and stores it in SQLite for fun & profit.

Please see [config.sample.edn](https://github.com/goshatch/money/blob/main/config.sample.edn) for information on how to setup categorization rules.

## Requirements

- [Babashka](https://github.com/babashka/babashka#installation) needs to be installed
- macOS or (I assume) Linux, *BSD, etc. Might be possible to adapt for Windows, but no guarantees there.

## Usage

Import transactions from CSV files:
```sh
mkdir -p ~/.config/money ~/.local/share/money
cp config.sample.edn ~/.config/money/config.edn
./money ~/Downloads/bank-export.csv ~/Downloads/credit-card-export.csv
```

Categorize transactions after the import (eg if you’ve updated your config file):

```sh
./money --categorize
```

## License

Copyright © 2024 Gosha Tcherednitchenko

[The GNU General Public License v3](https://www.gnu.org/licenses/gpl.html)

