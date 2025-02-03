# Expo Camera Multiple `onBarCodeScanned` Trigger Issue

This repository demonstrates a bug in Expo's `Camera` component where the `onBarCodeScanned` callback function is triggered multiple times for a single barcode scan.  This leads to unexpected behavior in applications that rely on this callback for actions such as making API calls or updating UI elements.

## Bug Reproduction

The `bug.js` file contains code that reproduces the issue.  Run the project and scan a barcode; observe that the console logs the barcode data multiple times.

## Solution

The `bugSolution.js` file provides a potential solution. This solution uses a debounce function to limit the number of times the `onBarCodeScanned` callback is executed within a short time frame.

## Contributing

Contributions are welcome!  If you have identified additional issues or alternative solutions, please submit a pull request.

## License

[MIT License](LICENSE)