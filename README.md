# Fuzzy-Implementation-with-Scikit-Fuzzy
# Fuzzy Home Heating System

## Problem Description

The objective of this project is to create a fuzzy logic system that determines the heating power of a home heating system. The system will adjust the heating power based on the following inputs:

- **Room Temperature (°C)**: Measures the current temperature of the room, ranging from 0°C to 40°C.
- **Desired Comfort Level**: Represents the desired comfort level for the occupants, ranging from "Very Cold" to "Very Warm."

### Output:
- **Heating Power (%)**: Represents how much power (0% to 100%) the heating system should use to adjust the room temperature to the desired level of comfort.

## Requirements

### Fuzzy Variables
1. **Room Temperature**: 
   - Cold
   - Comfortable
   - Hot

2. **Desired Comfort Level**:
   - Very Cold
   - Cold
   - Comfortable
   - Warm
   - Very Warm

3. **Heating Power**:
   - Low
   - Medium
   - High

### Membership Functions

- **Room Temperature**: Triangular or trapezoidal membership functions to model the fuzzy sets for cold, comfortable, and hot temperature ranges.
- **Desired Comfort Level**: Triangular or trapezoidal membership functions to represent the fuzzy sets for very cold, cold, comfortable, warm, and very warm comfort levels.
- **Heating Power**: Triangular or trapezoidal membership functions for low, medium, and high power settings.

### Fuzzy Rules

The fuzzy rules define how the system should react to different input conditions. Example rules include:

- If the room temperature is **cold** and the comfort level is **very warm**, then the heating power should be **high**.
- If the room temperature is **comfortable** and the comfort level is **comfortable**, then the heating power should be **medium**.
- If the room temperature is **hot** and the comfort level is **very cold**, then the heating power should be **low**.
- If the room temperature is **cold** and the comfort level is **warm**, then the heating power should be **medium**.
- If the room temperature is **hot** and the comfort level is **warm**, then the heating power should be **low**.

### Example Rule Set:

| Room Temperature | Desired Comfort Level | Heating Power |
|------------------|-----------------------|---------------|
| Cold             | Very Warm             | High          |
| Comfortable      | Comfortable           | Medium        |
| Hot              | Very Cold             | Low           |
| Cold             | Warm                  | Medium        |
| Hot              | Warm                  | Low           |

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/Hansaka2001/Fuzzy-Implementation-with-Scikit-Fuzzy.git
