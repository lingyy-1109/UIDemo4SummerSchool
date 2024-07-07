# UI Demo for Summer School

This is a simple PyQt5 application that allows users to load an image from their file system, display the image, and show a score for the image.

## Files

- `main.py`: The main script to run the application.
- `demo.py`: Contains the UI class definition generated by PyQt5's UI code generator (maybe PYUIC). You should edit the file by editing `demo.ui` and using PYUIC to generate it.
- `demo.ui`: Contains the UI class definition and can be edited by Qt Creator.

## Requirements

- Python 3.x
- PyQt5

## Installation
If you just want to run the code, you can follow the instructions below:
1. Clone the repository or download the source code.
2. Make sure you have Python 3.x installed.
3. Install the required packages using pip:

    ```sh
    pip install PyQt5
    ```

**However, if you want to edit the ui files, you are preferred to download the Qt Creator and PYUIC plugin in the PyCharm. You can first download PyCharm IDE and follow the link below:**
https://blog.csdn.net/qq_45041871/article/details/113775749

## Usage

1. Run the `main.py` script to start the application:

    ```sh
    python main.py
    ```

2. Click on the "Load a Picture" button to open a file dialog.
3. Select an image file (PNG, JPG, BMP).
4. The selected image will be displayed in the `PicLabel`.
5. A score will be calculated and displayed in the `ScoreLabel`.

## Code Overview

### main.py

This script contains the main application logic:

- **MainWindow Class**: Inherits from `QMainWindow` and `Ui_MainWindow`. The `__init__` method sets up the UI and connects the "Load a Picture" button to the `load_picture` function.
- **load_picture Function**: Opens a file dialog to select an image file. If a file is selected, it calls `show_picture` to display the image and `calculate_score` to compute and display the score.
- **show_picture Function**: Sets the selected image in the `PicLabel` using `QPixmap`.
- **calculate_score Function**: A placeholder function that returns a dummy score (42). Replace this with actual logic for calculating the score from the image.

### demo.py

This file contains the `Ui_MainWindow` class generated by PyQt5's UI code generator from the `demo.ui` file.


## License

This project is licensed under the MIT License.

## Copyright

版权所有 © 上海交通大学医疗机器人研究院郭遥课题组
