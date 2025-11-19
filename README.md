# validate-nric

Singapore NRIC/FIN validation tool - Run directly from GitHub Pages

## 🚀 Quick Start

**[👉 Open the app here](https://antloh-sh.github.io/validate-nric/)**

Or visit: `https://antloh-sh.github.io/validate-nric/`

## Features

- ✅ Format validation (S/T/F/G prefix + 7 digits + checksum letter)
- ✅ Checksum verification using weighted algorithm
- ✅ Supports both NRIC and FIN formats
- ✅ Clean, responsive UI built with Bootstrap
- ✅ Works entirely in the browser (no backend needed)
- ✅ Instant results with helpful error messages

## How It Works

1. Enter a Singapore NRIC or FIN number
2. The app validates the format
3. Calculates and verifies the checksum
4. Shows if the number is valid or not

### Valid Format
- **Prefix**: S, T, F, or G
- **Digits**: 7 digits
- **Checksum**: 1 letter (A-Z)
- **Example**: S1234567A, T9876543Z, F1111111A

## Files

- `index.html` - Complete app with HTML, CSS, and JavaScript
- `README.md` - This file

## Technology

- **Frontend**: HTML5, CSS3, Bootstrap 5, JavaScript
- **Hosting**: GitHub Pages
- **Validation**: Client-side JavaScript (no server needed)

## Validation Algorithm

The app uses Singapore's official NRIC/FIN checksum algorithm:
1. Extract the 7 digits from the NRIC/FIN
2. Apply weights [2, 7, 6, 5, 4, 3, 2] to each digit
3. Sum the weighted values
4. Calculate remainder: sum % 11
5. Map remainder to checksum letter using lookup table

## License

Open source - feel free to use and modify

## About

This tool was created for community service programs in Singapore to help validate member identification numbers.
