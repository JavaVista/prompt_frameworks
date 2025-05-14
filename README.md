# Prompt Frameworks

A practical guide and demonstration of different prompt engineering frameworks using Google's Generative AI.

## Features
- Implementation of prompting methodology
- Interactive Jupyter notebook examples
- Ready-to-use prompt templates
- Real-world use cases and examples

## Prerequisites
- Python 3.8+
- Google API key for Generative AI

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/prompt_frameworks.git
cd prompt_frameworks
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate # on Windows, use `venv\Scripts\activate`
```
3. Install the required packages:
```bash
pip install -r requirements.txt
```
## Configuration

1. Get your Google API key for Generative AI from [Google AI Studio](https://aistudio.google.com/).

2. Create a `.env` file in the root directory of the project.

3. Add the following line to the `.env` file:
```bash
GOOGLE_API_KEY=your_api_key_here
```
## Usage
1. Run the Jupyter notebook:
```bash
jupyter notebook # or jupyter lab
```
2. Open the `prompt_frameworks_presentation.ipynb` notebook and follow the instructions.

## Optional - Running the Jupyter Notebook as a HTML Slideshow with RISE

### Run the Classic Jupyter Notebook Interface

1. Launch the classic notebook interface from the terminal:

```bash
jupyter notebook
```
Firebase Studio will provide a public URL in the terminal output (e.g., ```http://localhost:8888/...```). Open it in the browser.

2. Once open, select prompt_frameworks_presentation.ipynb.

3. Click the RISE (bar chart) icon in the toolbar to start the slideshow.

**Note**: RISE currently works best in the classic notebook interface, not JupyterLab

### Export to Reveal.js HTML Slides
1. Convert the Jupyter notebook to a Standalone HTML slideshow using the `nbconvert` command-line tool:

```bash
jupyter nbconvert prompt_frameworks_presentation.ipynb --to slides --reveal-prefix https://unpkg.com/reveal.js@5.1.0/ --output presentation.html
```
2. Open the generated `prompt_frameworks_presentation.slides.html` file in a web browser to view the slideshow.

### Note for Firebase Studio / Project IDX Users
If you're using **Firebase Studio** or **Google Project IDX**, you may encounter the following error when running a cell in Jupyter Notebook:

```bash
Running cells with 'venv (Python 3.11.10)' requires the ipykernel package.
Run the following command to install 'ipykernel' into the Python environment. 
Command: '/home/user/prompt_frameworks/fwenv/bin/python -m pip install ipykernel -U --force-reinstall'
```
This is caused by the absence of the GNU C++ runtime library (`libstdc++.so.6`), which is required by native Python packages such as `pyzmq` used by Jupyter.

#### Solution
1. Open your `dev.nix` file (located at the root of your project).
2. Add `pkgs.gcc13` to the `packages` list:

```bash
{
 channel = "stable-24.05";

 packages = [
   pkgs.python311
   pkgs.python311Packages.pip
   pkgs.gcc13  # ✅ Adds libstdc++.so.6 needed for Jupyter
 ];

 env = {};

 ...
}
```
## Contact / Social Media

- Twitter – [@seetechnologic](https://twitter.com/seetechnologic)
- GitHub - [https://github.com/JavaVista/](https://github.com/JavaVista/)
- LinkedIn - [Javier Carrion](https://www.linkedin.com/in/technologic)
- Website - [techno-logic.us](https://www.techno-logic.us)

## License
This project is licensed under the MIT License.