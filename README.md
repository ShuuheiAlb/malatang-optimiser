# Malatang Optimiser

This Excel-based tool helps you build a better Malatang bowl - choosing ingredients and portion sizes that keep a good macro balance (protein, carbs, fat) and overall variety, while staying within your budget.

It's powered by Excel's Solver, so no coding required. You can adjust things like max weight, number of ingredients, and your preferred macro ratio - and it’ll suggest a combo that tries to balance all of that. Set your preference and hit Solve.

## Data Collection & Methodology

I pull the ingredient names from this site: [Maigoo – Malatang Ingredient List](https://m.maigoo.com/goomai/160395.html) which is then translated into English.

After that, I looked up the nutritional info manually for each item using
[China Food Nutrition Database](https://nlc.chinanutri.cn/fq/). For this part, no automation yet and still in progress — there’s a lot of veggie types. So the dataset isn’t perfect, but hopefully it’s enough to get the optimisation idea across.

If you’ve got cleaner data, feel free to plug it into the Excel and go wild.

Underneath it uses a simplified Lasso-style formula to juggle multiple priorities: how close the macro ratio is to your target, total weights and number of ingredients.

## Inspo

When you're building your Malatang bowl, it's super easy to overload on heavy ingredients like tofu or enoki mushrooms — and the grams (and price) really add up fast.

I want to create a simple Excel tool to help people optimise ingredient choices and portion sizes based on budget or dietary targets. Limitation is, I didn’t have access to super detailed ingredient data (exact weights, macros, prices, etc), but if you do - oh well, I’ve built the template so you can plug those in.
