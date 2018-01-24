# Budget

Example project from: https://www.codeschool.com/screencasts/build-a-bank-statement-cli-application-with-elixir

## Installation

If [available in Hex](https://hex.pm/docs/publish), the package can be installed
by adding `budget` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {:budget, "~> 0.1.0"}
  ]
end
```

Documentation can be generated with [ExDoc](https://github.com/elixir-lang/ex_doc)
and published on [HexDocs](https://hexdocs.pm). Once published, the docs can
be found at [https://hexdocs.pm/budget](https://hexdocs.pm/budget).

## What this does

1. Reads a CSV

```
AcctNum,TranDate,Description,Amount
4002617,01/01/2017,Rent,-1000.00
4002617,01/03/2017,Netflix,-9.99
4002617,01/03/2017,Credit Card,-538.00
4002617,01/04/2017,Car Payment,-320.01
4002617,01/04/2017,Publix,-53.39

```

2. Filters out the account number

3. Normalizes the amounts (string to float)

4. Formats the result for display

```
Transactions:
01/03/2017 Netflix 		$9.99
01/04/2017 Publix 		$53.39
01/04/2017 Car Payment 	$320.01
01/03/2017 Credit Card 	$538.00
01/01/2017 Rent 		$1000.00
```