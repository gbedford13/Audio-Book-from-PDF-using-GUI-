# Audio-Book-from-PDF-using-GUI-
PDF to Audiobook Converter
A simple Python GUI application that converts a PDF file into an audiobook MP3 file. The app uses Tkinter for the graphical interface, PyPDF2 to extract text from PDFs, and gTTS to convert the extracted text into speech.
Features


Select a PDF file using a graphical file picker


Extract text from all pages of the PDF


Convert extracted text into speech


Save the audiobook as an MP3 file


Automatically open/play the generated MP3 file


Error handling for missing files or conversion issues


Technologies Used


Python


Tkinter


gTTS


PyPDF2


OS module


Requirements
Make sure Python is installed on your computer.
Install the required Python packages:
pip install gTTS PyPDF2
Tkinter usually comes pre-installed with Python. If it is missing, install it based on your operating system.
How to Run


Save the Python code in a file, for example:


pdf_to_audiobook.py


Run the program:


python pdf_to_audiobook.py


A small window will open.


Click the Convert PDF to Audiobook button.


Choose a PDF file from your computer.


The program will extract the text, convert it to speech, and save the MP3 file in the same folder as the selected PDF.


Output
The generated audiobook will be saved using the original PDF filename with _audiobook.mp3 added.
Example:
mybook.pdf
will become:
mybook_audiobook.mp3
Project Structure
PDF-to-Audiobook/│├── pdf_to_audiobook.py└── README.md
How It Works
The program opens a GUI window using Tkinter. When the user clicks the button, a file dialog appears so the user can select a PDF file. The PDF is read using PyPDF2, and text is extracted page by page. The extracted text is then passed to gTTS, which converts it into an MP3 audiobook file.
Notes


This program works best with PDFs that contain selectable text.


Scanned PDFs or image-only PDFs may not work because PyPDF2 cannot extract text from images.


An internet connection is required because gTTS uses Google Text-to-Speech.


os.startfile() works on Windows. For macOS or Linux, a different method may be needed to open the MP3 automatically.


Possible Improvements


Add support for scanned PDFs using OCR


Allow the user to choose the output folder


Add language selection


Add progress bar during conversion


Support macOS and Linux audio playback


Split long PDFs into multiple audio files


License
This project is open source and available for educational use.
