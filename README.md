# Rental Price Predictor

This is one of my beginner Python projects. I made it to practice lists, dictionaries, functions, and simple logic by predicting apartment rent from rooms, bathrooms, and area.

## Why I made this
I wanted to build a small project that is easy to understand but still feels useful. Instead of making only basic print programs, I tried creating something that takes real-looking rental data and gives a rent prediction.

## What this project does
- Stores sample apartment data
- Prints rental listings in a clean format
- Predicts rent for a new apartment
- Uses a simple formula based on rooms, bathrooms, and area

## Formula used
The program uses this formula:

`Rent = (rooms * 5000) + (bathrooms * 3000) + (area * 20)`

For example:
- Rooms: 2
- Bathrooms: 1
- Area: 850 sqft

Predicted rent:
`₹30,000/month`

## Tech used
- Python 3
- VS Code
- GitHub

## Project files
```bash
Rental-Price-Predictor/
├── rental_predictor.py
└── README.md
```

## Python code
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

## Sample output
```text
Rental Data:
1BHK, 1bath, 500sqft: ₹15,000
2BHK, 1bath, 800sqft: ₹25,000
3BHK, 2bath, 1200sqft: ₹40,000

Predicted: 2BHK, 1bath, 850sqft = ₹30,000/month
```

## How to run it
1. Make sure Python 3 is installed.
2. Download or clone this repository.
3. Open the folder in VS Code or terminal.
4. Run this command:

```bash
python rental_predictor.py
```

## What I learned
While making this project, I practiced:
- Python dictionaries and lists
- Functions
- Looping through data
- Formatting output
- Writing a small project and uploading it to GitHub

## Future improvements
- Add more apartment data
- Take user input instead of fixed values
- Improve the prediction logic
- Turn it into a small web app later

## Author
Danish Dhammani  
BCA 2nd Year Student  
Learning Python and building beginner projects


 
