# Persona Chef: Your Personal Recipe Assistant

## Overview

Persona Chef is an intelligent recipe assistant that personalizes cooking recommendations based on your preferences, dietary restrictions, and available ingredients. Whether you're a seasoned chef or a cooking novice, Persona Chef adapts to your unique culinary persona to provide tailored recipe suggestions, cooking tips, and meal planning assistance.

## Features

- **Personalized Recipe Recommendations**: Get recipe suggestions based on your taste preferences, cooking skill level, and dietary needs
- **Ingredient-Based Search**: Find recipes using ingredients you already have in your kitchen
- **Dietary Restriction Support**: Easily filter recipes for various diets (vegan, gluten-free, keto, etc.)
- **Meal Planning**: Generate weekly meal plans optimized for your preferences and nutritional goals
- **Step-by-Step Guidance**: Receive clear cooking instructions with timing estimates for each step
- **Cooking Tips**: Learn techniques and substitutions personalized to your skill level
- **Favorite Collections**: Save and organize recipes you love for quick access

## How It Works

The Persona Chef system uses a combination of machine learning algorithms and nutritional databases to create a personalized cooking experience:

1. **User Profiling**: Creates a culinary persona based on your preferences, restrictions, and cooking habits
2. **Recipe Matching**: Uses collaborative filtering and content-based recommendation algorithms to find recipes that match your profile
3. **Ingredient Analysis**: Analyzes your available ingredients to suggest recipes that minimize waste and shopping needs
4. **Nutritional Optimization**: Ensures meal plans meet your nutritional requirements while respecting your taste preferences

## Jupyter Notebook Implementation

The `personal_chef.ipynb` notebook demonstrates the core functionality of the Persona Chef system:

- Data preprocessing of recipe datasets
- User preference modeling
- Recipe recommendation algorithms
- Nutritional analysis
- Meal plan generation

## Getting Started

### Prerequisites

- Python 3.8+
- Jupyter Notebook
- Required Python libraries (pandas, scikit-learn, numpy, matplotlib)

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/persona-chef.git
   cd persona-chef
   ```

2. Install required packages:
   ```
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:
   ```
   jupyter notebook
   ```

4. Open `personal_chef.ipynb` to explore the implementation

## Example Usage

```python
# Create a user profile
user_profile = PersonaChef.create_profile(
    preferences=["Italian", "Mexican", "Thai"],
    restrictions=["vegetarian"],
    cooking_time=30,  # minutes
    skill_level="intermediate"
)

# Get personalized recipe recommendations
recommendations = user_profile.get_recommendations(top_n=5)

# Generate a meal plan for the week
meal_plan = user_profile.generate_meal_plan(
    days=7,
    meals_per_day=3,
    calories_per_day=2000
)

# Find recipes with available ingredients
available_ingredients = ["chicken", "rice", "bell peppers", "onions", "garlic"]
matching_recipes = user_profile.find_recipes_by_ingredients(available_ingredients)
```

## Data Sources

- Recipe data from [Food.com](https://www.food.com/)
- Nutritional information from [USDA FoodData Central](https://fdc.nal.usda.gov/)
- Ingredient substitutions from [The Cook's Thesaurus](http://www.foodsubs.com/)

## Future Enhancements

- Integration with grocery delivery services
- Voice-activated recipe guidance
- Image recognition for ingredient identification
- Social sharing and community recipe ratings
- Seasonal and local ingredient recommendations

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Recipe data providers
- Nutritional database contributors
- Open source machine learning libraries

---

*Bon Appétit with your personal culinary companion!*
