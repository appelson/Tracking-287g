## Note
This project was created in my personal capacity. Should you have any questions or suggestions for other public immigration data you would like to see tracked, you can contact me at elijahappelson@gmail.com. 

# Tracking 287(g)

This repository downloads data from the **287(g)** program and organizes it to be used by journalists, advocates, and the public. The scraper runs daily, extracting data from the official [ICE 287(g) page](https://www.ice.gov/identify-and-arrest/287g). The data is saved in two main folders:

- **`agreements/`**: Contains PDFs of all 287(g) agreements between law enforcement agencies and ICE, categorized by download date/time, state, and agency.
- **`sheets/`**: Stores Excel files listing participating and pending agencies, as published on the ICE website, categorized by download date/time.

## Purpose

Law enforcement agencies are increasingly entering into agreements with ICE under the **287(g)** program, assisting in the deportation of immigrants from across the U.S. This program is supported by mandates like [Louisiana Executive Order Number JML 25-060: Project Geaux](https://interactive.wwltv.com/pdfs/Operation_GEAUX.pdf), which directs state law enforcement agencies to collaborate with ICE.

As mandates like this continue to grow, it’s crucial to track which agencies are involved in the program. This provides a real-time overview of participating agencies and their respective agreements.

## Setup

To use this repository, follow these steps:

### 1. Clone the repository
Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/tracking-287g.git
```

### 2. Install dependencies
Ensure you have Python installed on your system. Then, install the necessary dependencies by running:

```bash
pip install -r requirements.txt
````
### 3. Run the scraper
To start the scraper, run the following command:

```bash
python scraper.py
```

## File Structure

- `.github/workflows/run_scripts.yaml`: GitHub Actions workflow file used for automating the execution of the scraper script.
- `scraper.py`: The Python script responsible for scraping 287(g) data from the ICE website.
- `agreements/`: Directory that stores the PDF agreements between ICE and law enforcement agencies.
- `sheets/`: Directory that stores the excel files with data on participating and pending agreements between ICE and law enforcement agencies.
- `requirements.txt`: Text file listing all Python dependencies required to run the scraper.
- `README.md`: This file.
