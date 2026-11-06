# Using Offline Recipe Scaling Kit

## Quick start

Run `./recipe-kit examples/recipe.json 6`. JSON contains `title`, positive `servings`, and `ingredients` with name/quantity/unit. Output goes to stdout; the input remains unchanged.

## Supported workflow

1. Structured JSON recipe scaling.
2. Fractional quantities without intermediate rounding.
3. Validated servings and unchanged ingredient units.

## Validation and troubleshooting

Run the commands in the README. Invalid inputs produce explicit errors rather than silently changing the requested operation. Browser audio requires a user gesture; microphone apps require HTTPS or localhost and permission. For file tools, supply supported input formats and writable output directories.

## Limitations

Does not convert units, infer cooking times, or assess allergens/nutrition. Scaling cooking technique requires judgement.

Tests use synthetic fixtures. These tests do not certify hardware compatibility, real-world forecast quality, trained-model accuracy, or production suitability for every input.
