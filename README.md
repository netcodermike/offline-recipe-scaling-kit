# Offline Recipe Scaling Kit

Scale structured ingredient quantities and servings without rounding intermediate measurements.

**Language:** Swift · **License:** MIT · **Data:** Local by default

## What it does

- Structured JSON recipe scaling
- Fractional quantities without intermediate rounding
- Validated servings and unchanged ingredient units

## Requirements

Swift 5.9 or newer (macOS or Linux toolchain).

## Install, validate, and run

```sh
swiftc main.swift -o recipe-kit
./recipe-kit --self-test
./recipe-kit examples/recipe.json 6
```

Run `--help` where supported, or follow the examples in [docs/usage.md](docs/usage.md). Input files are never overwritten unless explicitly documented.

## Usage and examples

See [docs/usage.md](docs/usage.md) for a walkthrough and [docs/architecture.md](docs/architecture.md) for implementation details. Tests are deterministic and do not require an exchange, paid API, external model, microphone, or private data.

## Boundaries

Does not convert units, infer cooking times, or assess allergens/nutrition. Scaling cooking technique requires judgement.

## Privacy

No analytics or accounts are built in. Local file tools process only the paths you supply. For model-server and weather apps, the interface and usage guide identify the destination and the data sent. Do not commit personal input files, model credentials, or generated recordings.

## Development

Run the validation commands above before submitting changes. GitHub Actions runs these checks on pushes and pull requests. See the workflow for the reproducible toolchain. A successful workflow verifies the tested paths; manual audio-device behavior is documented separately.
