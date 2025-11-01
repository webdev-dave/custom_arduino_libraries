# Custom Arduino Libraries

Personal collection of custom Arduino libraries. Only folders prefixed with `Custom_` (case-insensitive) are tracked.

## Installation

1. **Clone this repository:**

```bash
git clone https://github.com/yourusername/your-repo-name.git
```

2. **Find your Arduino libraries folder:**

   The location varies depending on your setup. The easiest way to find it:

   - Open an existing Arduino project (`.ino` file) in your file explorer
   - Go up one level to see the project folder
   - Go up one more level - you should see a `libraries` folder

   Default locations (if you haven't changed them):

   - Windows: `Documents\Arduino\libraries\`
   - Mac: `~/Documents/Arduino/libraries/`
   - Linux: `~/Arduino/libraries/`

3. **Copy to Arduino libraries folder:**

   Copy all `Custom_*` folders from the cloned repository into your `libraries` directory.

4. **Restart Arduino IDE**

## Usage

Include libraries in your sketch using the header file name:

```cpp
#include <pitches.h>      // From Custom_Pitches folder
#include <myutils.h>      // From Custom_MyUtils folder
```

## Adding New Libraries

1. Create a new folder with `Custom_` prefix (e.g., `Custom_Sensors`)
2. Add your `.h` and/or `.cpp` files inside
3. Optionally add `library.properties` for metadata
4. Commit and push to this repo

**Example structure:**

```
Custom_MyLibrary/
├── mylibrary.h
├── mylibrary.cpp           (optional)
└── library.properties      (optional)
```
