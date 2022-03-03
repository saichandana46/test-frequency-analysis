# Title: Simple Frequency Analysis on user-supplied text.

# Description:

- This application reads a user supplied text file and counts the frequencies of the words in it.
- The top 25 most frequently repeated words are reported.
- Non-letter characters are ignored from the text.
- Ability to read a stopwords file, user can decide if they want to exclude or include stopwords in the original text.
- User can decide to perform stemming of the words(replace/remove suffixes according to the given grammar rules).

  ** Grammar Rules:

  - The following are common suffixes in the language, remove the suffix to find the root word -

    - “L”
    - “LZ”
    - “EVM”
    - “ZQ”

  - These suffixes require adding back letters to determine the root word -

    - remove “ZL” add “A”
    - remove “PZL” add “AZ”
    - remove “EZL” add “R”

- Perform lookups in the original text using stems, extracting root words and their inflections.
- Output is exported to a directory in the current working directory.
- Creates a nested folder structure with a timestamp attached to the subfolder name under folder output.
- Each subfolder includes originaltext file and results file.
- For example, the output structure looks like:
  - output/
    analysis-2022-03-02_16-48-52/
    originaltext.txt
    results.txt

# How to install and run the project:

- Download the zipped repo
- This is a python based project
- Install Python version 3.6+, Current Python version I used is Python 3.8.12
- Python Libraries involved: json, re, os, datetime, collections, typing
- (Optional) If required create a virtual environment, using the cmd prompt
  Command to create: python3 -m venv venv
  To activate: source venv/bin/activate
  To deactivate: deactivate
- To run the app, use python3 analysis.py
- Then supply input text file, stopwords text file, apply settings according to the input prompt
- Results are exported to the file

<!-- Hours spent on this exercise - 8 hours -->

