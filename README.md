# Tool-to-Generate-Synthetically-Warped-Document-Images

This tool is used to generate synthetically warped document images. It provides an interface for uploading an image, applying various effects to it, and exporting the modified image.

## Installation

To run this tool, follow these steps:

1. **Ensure you have Python installed** on your system. You can download Python from the official website: [Python.org](https://www.python.org/downloads/).

2. **Clone this repository** to your local machine using Git or download the code as a ZIP file and extract it.

3. **Navigate to the 'app' directory** on your command line/terminal.

4. **Install the required Python libraries** by running the following command:

    ```
    pip install -r requirements.txt
    ```

   This will install all the necessary dependencies, including PyQt5, qtawesome, and other libraries used by the app.

5. Make sure you have **Blender installed** on your system. You can download Blender from the official website: [Blender.org](https://www.blender.org/download/).

6. Once the dependencies are installed, you can **run the app** by executing the following command in the 'app' directory:

    ```
    python mainwindow.py
    ```

   This will launch the tool.

In case you face issues with installation of some dependencies, follow these steps to setup a virtual environment

1. **Navigate to the app directory of this project and install pyenv-win in PowerShell** using command:
    ```
    Invoke-WebRequest -UseBasicParsing -Uri "https://raw.githubusercontent.com/pyenv-win/pyenv-win/master/pyenv-win/install-pyenv-win.ps1" -OutFile "./install-pyenv-win.ps1"; &"./install-pyenv-win.ps1"
    ```

2. **Reopen PowerShell** and check pyenv version with the following command:
    ```
    pyenv --version
    ```
    
3. **Install python** version bundled with your blender software
    ```
    pyenv install 3.10.2
    ```
    
    **Note:** Python 3.10 series is supported in Blender 3.5. To check python version bundled with your Blender version, open blender and navigate to its console or press ctrl+alt+shift+P and run the following command: 
    ```
    import sys
    print(sys.version_info[:3])
    ```
    This will print the Python version.

4. **Activate virtual environment**
     ```
     python -m venv myenv
     myenv\Scripts\activate
     ```

5. **Run the project**
     ```
     pip install -r requirements.txt
     python mainwindow.py
     ```

This will launch the project.

## Usage

1. Upon launching the app, you will see the main window with an **"Upload Image"** button.

2. Click the **"Upload Image"** button to select an image file (in PNG, JPG, or JPEG format) from your local machine.

3. Once the image is uploaded, you can choose from various effects such as **"Curved," "Perspective Shift," "One Fold,"** etc. by clicking the corresponding buttons.

4. The selected effect will be applied to the uploaded image, and the modified image will be displayed in the app window.

5. You can **save the modified image as a PNG file** by clicking the **"Save File as PNG"** button.

6. Additionally, you can **export the modified image to a Blender file** by clicking the **"Export to Blender File"** button. This will generate a Blender file with the applied effect.

7. To exit the app, simply **close the main window**.

Feel free to explore and experiment with different effects using this tool!
