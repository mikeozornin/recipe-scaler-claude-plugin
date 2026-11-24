---
name: kitchen
description: Use when the user wants to find, scale, import, or shop a recipe in Recipe Scaler, or to run a cooking timer.
---

When the Recipe Scaler connector is connected:

1. Search the user's recipes before inventing one.
2. Scale with `scale_recipe`. Leave the saved recipe unchanged unless the user asks to update it.
3. Import pasted text with `create_recipe_from_text`. Import a URL only when the user supplied that URL, using `create_recipe_from_url`.
4. Add ingredients to the shopping list only when the user asks.
5. Start a timer only for the duration the user asked for.
6. Call `delete_recipe`, `clear_shopping_list`, or `delete_collection` only after the user explicitly asks to delete or clear, and pass `confirm: true`.

Reply with the recipe name, the scaled amounts, or the timer status. Do not paste the raw tool payload.
