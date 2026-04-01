# Rental-Price-Predictor

A simple Python project that predicts apartment rent using rooms, bathrooms, and area data.

## Overview
This project is a beginner-friendly rental price prediction program built in Python.  
It stores sample rental property data and uses a custom formula to estimate rent for a new property.

## Features
- Stores rental property data in Python dictionaries
- Displays sample rental listings
- Predicts rent using rooms, bathrooms, and area
- Built using pure Python without external libraries

## Technologies Used
- Python 3
- VS Code
- GitHub

## Project Structure
```bash
Rental-Price-Predictor/
│── rental_predictor.py
│── README.md
```

## How It Works
The program uses this formula to estimate rent:

`Rent = (rooms * 5000) + (bathrooms * 3000) + (area * 20)`

Example:
- Rooms = 2
- Bathrooms = 1
- Area = 850 sqft

Predicted Rent = ₹30,000/month

## Sample Code
```python
rentals = [
    {"rooms": 1, "bathrooms": 1, "area": 500, "price": 15000},
    {"rooms": 2, "bathrooms": 1, "area": 800, "price": 25000},
    {"rooms": 3, "bathrooms": 2, "area": 1200, "price": 40000}
]

print("Rental Data:")
for rental in rentals:
    print(f"{rental['rooms']}BHK, {rental['bathrooms']}bath, {rental['area']}sqft: ₹{rental['price']:,}")

def predict_rent(rooms, bathrooms, area):
    return (rooms * 5000) + (bathrooms * 3000) + (area * 20)

new_rental = predict_rent(2, 1, 850)
print(f"\nPredicted: 2BHK, 1bath, 850sqft = ₹{new_rental:,}/month")
```

## Sample Output
```text
Rental Data:
1BHK, 1bath, 500sqft: ₹15,000
2BHK, 1bath, 800sqft: ₹25,000
3BHK, 2bath, 1200sqft: ₹40,000

Predicted: 2BHK, 1bath, 850sqft = ₹30,000/month
```

## How to Run
1. Install Python 3
2. Download or clone this repository
3. Open the project folder in VS Code
4. Run:

```bash
python rental_predictor.py
```

## Future Improvements
- Add more rental data
- Improve prediction formula
- Build a graphical interface
- Convert it into a web-based rent predictor

## Author
**Danish Dhammani**  
BCA Student | Python Learner | Aspiring Software Developer
