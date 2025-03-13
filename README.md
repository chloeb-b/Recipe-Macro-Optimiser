# Recipe Macro Optimiser

A multi-objective meal planning system that balances nutritional goals with user taste preferences using genetic algorithms.

## Overview

In recent years, there has been an increase in the number of healthy recipe platforms, nutrition applications, and diet-focused research. To make use of this wealth of information, computational solutions for meal planning have emerged, selecting from central databases of healthy recipes. However, these computational solutions are often impersonalized to users' taste preferences.

This project endeavors to refine the flexibility of meal plan recommender systems by balancing the objectives of nutritional goals and recipe preferences. Nutritional meal plans are optimized from user-personalized recipe collections, creating preference-aware suggestions. Not everyone is a nutritionist, and some individuals don't mind making partial sacrifices in nutritional goals if they can continue to enjoy the foods they love.

The technical focus and novelty of this project is the development of dynamic, user-driven models for wide ranges of nutritional objectives and taste preferences. Ultimately, we aim to produce a recommender system that can be utilized to generate meal plans that are both nutritional and highly personalized.

## Features

- Multi-objective optimization using genetic algorithms
- User preference weighting system
- Support for different diet types (balanced, low-fat, low-carb, high-protein)
- Interactive GUI for user input and meal plan visualization
- Personalized recipe recommendations based on user ratings
- Macro nutrient optimization (protein, fat, carbohydrates)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Recipe-Macro-Optimiser.git
cd Recipe-Macro-Optimiser
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate
```

3. Install the required packages:
```bash
pip install -r requirements.txt
```

4. Create a `.env` file in the project root and add your RapidAPI key:
```
RAPIDAPI_KEY=your_api_key_here
```

## Usage

1. Run the demo notebook:
```bash
jupyter notebook demo.ipynb
```

2. Follow the interactive prompts to:
   - Enter your personal details (age, gender, height, weight)
   - Select your activity level
   - Choose your weight goal
   - Set your preference for taste vs. nutritional goals

3. The system will generate a personalized meal plan based on your inputs and preferences.

## Project Structure

- `demo.ipynb`: Main notebook containing the application logic
- `requirements.txt`: List of Python dependencies
- `nutr_df.csv`: Nutritional data for recipes
- `recipe_meta.csv`: Recipe metadata
- `reduced_train.csv`: Training data for recipe recommendations
- `all_user_ids.csv`: User IDs for the system

## Technical Details

The system uses:
- Genetic algorithms for multi-objective optimization
- PyQt5 for the graphical user interface
- Pandas and NumPy for data manipulation
- Matplotlib for visualization
- RapidAPI for nutritional calculations

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Recipe data and images are sourced from AllRecipes
- Macro targets are calculated using the RapidAPI Fitness Calculator API (https://rapidapi.com/malaaddincelik/api/fitness-calculator)