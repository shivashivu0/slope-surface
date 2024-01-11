
# SlopeSurface Smart Contract

This Solidity smart contract, named `SlopeSurface`, provides functions for calculating momentum and determining the position of a body on a slope surface. The contract utilizes the SafeMath library for secure mathematical operations.

## Functions

### 1. `calculateMomentum`

Calculates the momentum of a body on a slope surface based on its mass and angle.

**Parameters:**
- `mass_`: Mass of the body in kilograms.
- `angle`: Angle of the slope in degrees.

**Conditions:**
- Requires the angle to be greater than 25 degrees, indicating that the body will slide.
- Asserts that the mass is greater than 10.

**Returns:**
- Calculated momentum of the body.

### 2. `bodyPosition`

Determines the position of a body on a slope surface based on its mass.

**Parameter:**
- `mass`: Mass of the body in kilograms.

**Conditions:**
- If the mass is less than or equal to 50, no specific action is taken.
- If the mass is greater than 50, reverts the transaction with the message "Body will continue to roll."

## Dependencies

The contract relies on the OpenZeppelin SafeMath library to perform secure mathematical operations, ensuring protection against overflow and underflow vulnerabilities.


## Usage

Deploy the `SlopeSurface` contract to a compatible blockchain network, and interact with its functions as needed. Be mindful of the conditions specified in each function to ensure proper usage.

## License

This contract is released under the MIT License. See the `LICENSE` file for details.
