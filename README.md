# Rental-Price-Predictor

Python project that predicts apartment rent using rooms, bathrooms, and area data.

## Features
- Stores rental property data
- Predicts rent using a simple formula
- Built using pure Python without external libraries

## Code
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

Predicted: 2BHK, 1bath, 850sqft = ₹25,000/month
```

## Author
Danish Dhammani
