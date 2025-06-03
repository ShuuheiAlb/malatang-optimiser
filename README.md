# Malatang Optimiser

This file lets you build a better Malatang bowl by choosing ingredients and portion sizes that maintain good macro balance (protein, carbs, fat) and overall variety while staying within your budget.

It's powered by Excel's Solver, so no coding required! You can adjust parameters like maximum weight, number of ingredients, and your preferred macro ratio, and it’ll suggest the combination of portions that balance all of that.

## Data Collection & Methodology

**Ingredient Data:**
I sourced ingredient names from [Maigoo – Malatang Ingredient List](https://m.maigoo.com/goomai/160395.html), then translated them into English.

**Nutritional Information:**
I manually collected each ingredient data using the [China Food Nutrition Database](https://nlc.chinanutri.cn/fq/). This process isn't automated yet and is still in progress - there are still many vegetable varieties to cover. So the dataset isn't perfect, but hopefully it's enough to get the optimisation concept across.

**Optimisation Algorithm:**
This uses a simplified Lasso-style formula to balance multiple priorities:
- Macro ratio proximity to your target
- Total weight constraints
- Number of ingredient variety

*If you’ve got cleaner data, feel free to plug it into the Excel template and experiment!*

## How to Use

1. Open the Excel file
2. Adjust your preferences:
   - Maximum total weight
   - Number of ingredients desired
   - Target macro ratio (protein:carbs:fat)
   - Budget constraints
3. Run Excel's Solver
4. Review the optimized ingredient selection and portions

## Inspiration

When building a Malatang bowl, it's easy to overload on heavy stuff like tofu or enoki mushrooms - and the weight (and thus cost) can ramp up really quickly.

I wanted to create an optimisation solution for this common problem. While I didn't have access to detailed ingredient data (exact weights, macros, prices), I've built a flexible template that can accommodate better data sources in case available.
