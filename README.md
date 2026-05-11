# Smart Waste Segregation System

## 📌 Description
This project is an automated system designed to identify and sort waste into four categories: Dry, Wet, Hazardous, and E-waste. 

## 🎯 Objectives
* To identify different categories of waste materials.
* To help users dispose of waste correctly using a 4-bin system.
* To reduce improper waste disposal.
* To promote recycling and environmental cleanliness.
* To create awareness about hazardous and electronic waste.
* To support smart city waste management systems.

## 🚀 Features
* **4-Bin System:** Separate bins for Dry, Wet, Hazardous, and E-waste.
* **Automatic Detection:** Uses sensors to categorize waste.
* **Real-time Processing:** Python-based logic for instant sorting.

  ## ⚙️ How It Works

* **Step 1: Input** – The user enters the name of the waste item into the system interface.
* **Step 2: Analysis** – The Python program checks the item against a pre-defined waste category database.
* **Step 3: Identification** – The system identifies if the item is **Dry, Wet, Hazardous, or E-waste**.
* **Step 4: Selection** – The correct bin for disposal is suggested to the user automatically.
* **Step 5: Instruction** – Specific disposal instructions are displayed to ensure safe handling.

  ![System Design](https://github.com/MeruguSrujana/smart-waste-segregation-system/blob/main/file_000000001b1c7207baff0039d25d0eea.png?raw=true)
  ## 💻 Project Code
<details>
<summary>▶ Click here to view the Full Python Code</summary>

```python
# ♻️ Smart Waste Segregation System
# Waste database for 4-bin segregation
waste_data = {
    "banana peel": {"category": "Wet Waste", "bin": "Green Bin", "message": "Can be used for composting."},
    "vegetable waste": {"category": "Wet Waste", "bin": "Green Bin", "message": "Biodegradable waste."},
    "food waste": {"category": "Wet Waste", "bin": "Green Bin", "message": "Suitable for compost preparation."},
    "paper": {"category": "Dry Waste", "bin": "Blue Bin", "message": "Can be recycled."},
    "plastic bottle": {"category": "Dry Waste", "bin": "Blue Bin", "message": "Send for recycling."},
    "cardboard": {"category": "Dry Waste", "bin": "Blue Bin", "message": "Reusable and recyclable material."},
    "battery": {"category": "Hazardous Waste", "bin": "Red Bin", "message": "Do not dispose with normal household waste."},
    "medicine": {"category": "Hazardous Waste", "bin": "Red Bin", "message": "Dispose safely to avoid contamination."},
    "chemical": {"category": "Hazardous Waste", "bin": "Red Bin", "message": "Handle carefully and avoid direct contact."},
    "charger": {"category": "E-Waste", "bin": "Black Bin", "message": "Electronic waste should be recycled separately."},
    "mobile phone": {"category": "E-Waste", "bin": "Black Bin", "message": "Contains electronic components for recycling."},
    "wire": {"category": "E-Waste", "bin": "Black Bin", "message": "Dispose at e-waste collection centers."}
}

print("♻️ SMART WASTE SEGREGATION SYSTEM ♻️")
print("-----------------------------------")

while True:
    item = input("\nEnter waste item: ").lower()

    if item in waste_data:
        print("\nWaste Identified Successfully")
        print("-----------------------------------")
        print("Waste Type :", waste_data[item]["category"])
        print("Put in     :", waste_data[item]["bin"])
        print("Suggestion :", waste_data[item]["message"])
    else:
        print("\nItem not found in database.")
        print("Please enter a valid waste item.")

    choice = input("\nDo you want to continue? (yes/no): ").lower()
    if choice != "yes":
        print("\nThank You for Using Smart Waste Segregation System")
        break
```

## 📊 Sample Output

<summary>Click to view the system in action</summary>


* **Waste Item Entered:** `battery`
* **Status:** Waste Identified Successfully
* **Category:** Hazardous Waste


---

## ✅ Conclusion
The **Smart Waste Segregation System** is a Python-based project designed to help users identify and sort waste efficiently. By categorizing items into specific bins, it promotes environmental sustainability and ensures hazardous materials are handled correctly.



