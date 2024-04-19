# GTA Math

## Introduction
GTA Math is a C++ library designed to handle matrix operations for Grand Theft Auto (GTA) game development. It provides functionalities for manipulating matrices, performing transformations, and managing render matrices within the game engine.

## Features
- Matrix attachment and detachment
- Matrix transformation operations
- Conversion between different matrix representations
- Update functions for RW (RenderWare) matrices
- Setting scale, rotation, and translation for matrices
- Handling matrix arithmetic operations

## Usage
To use the GTA Math library in your GTA game development project, follow these steps:

1. Clone or download the repository.
2. Include the necessary header file `StdInc.h` in your project.
3. Utilize the provided `CMatrix` class to perform matrix operations as needed.

## Example
```cpp
#include "StdInc.h"

// Example code demonstrating the usage of GTA Math library
int main() {
    // Create a new matrix
    CMatrix matrix;

    // Set translation
    matrix.SetTranslate(10.0f, 5.0f, 0.0f);

    // Perform rotation around Z axis
    matrix.SetRotateZOnly(90.0f);

    // Apply scale transformation
    matrix.SetScale(2.0f);

    // Update RW matrix
    matrix.UpdateRW();

    return 0;
}
```

## Development and Credits
- Frooze (SA Export and Reverse Engineering, Lead)
- JaneStar (Middleware Specialist)
- xcoey (Testing while development progress)
