# ReportsGenerator

Report generator that receives a .csv order file on iFood and returns the food and the user who asked for the most, adding up the total spent on each one.

## Installation

If [available in Hex](https://hex.pm/docs/publish), the package can be installed
by adding `reports_generator` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {:reports_generator, "~> 0.1.0"}
  ]
end
```

## Usage

```bash
$ ìex -S mix
```

### get Higher Value by user:
```elixir
"report_complete.csv"
|> ReportsGenerator.build()
|> ReportsGenerator.fetch_higher_value("users")
```

### get Higher value by food:
```elixir
"report_complete.csv"
|> ReportsGenerator.build()
|> ReportsGenerator.fetch_higher_value("foods")
```

## Test
```bash
$ mix test
```

Documentation can be generated with [ExDoc](https://github.com/elixir-lang/ex_doc)
and published on [HexDocs](https://hexdocs.pm). Once published, the docs can
be found at [https://hexdocs.pm/reports_generator](https://hexdocs.pm/reports_generator).

