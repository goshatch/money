# Money

> But if you ask for a rise<br/>
> It’s no surprise that they’re giving none away
>
> — Pink Floyd, _Money_

A personal finance manager. Work **very much** in progress.

Loads transaction data from banking export CSVs, normalizes the data, and stores it in SQLite for fun & profit.

Usage:

```sh
mkdir -p ~/.config/money ~/.local/money
cp config.sample.edn ~/.config/money/config.edn
./money ~/Downloads/bank-export.csv ~/Downloads/credit-card-export.csv
```

## License

Copyright © 2024 Gosha Tcherednitchenko

[The GNU General Public License v3](https://www.gnu.org/licenses/gpl.html)

