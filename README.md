
🧹 # Sales Data Cleaner 
1. 📌 Project Title & Goal

This project reads a messy sales CSV file, cleans the data, removes duplicates, converts prices from USD to INR, and generates a clean JSON report.

The entire project is implemented and executed in Google Colab using a Jupyter Notebook.

## 2. Setup Instructions
1.Open the notebook:
sales.clean.ipynb

2.Upload the CSV file:
sales.csv

3.Install required library (if not already installed):
pip install pandas

4.Run all the cells in the notebook.

After successful execution, a file named:
clean_file.json will be generated.

## 3. The Logic (How I thought)

### Why did I choose this approach?
I used the Pandas library because it makes data cleaning, transformation, and file conversion very easy and efficient. It is widely used in  Data Science tasks.

### What was the hardest bug you faced, and how did you fix it?
The main issue was that the JSON file was getting saved in a different folder in Google Colab. I fixed this by giving the correct file path while saving the JSON file, so now it is saved in the same working directory.

### Steps:
- Read CSV file using pandas
- Removed $ sign and quotes from price column
- Converted price to float
- Removed duplicate rows based on product and price
- Converted USD price to INR (1 USD = 83 INR)
- Saved the final clean data to `clean_sales.json`

## 4. Output Screenshots

### ✅ Script Running Successfully
![Script Output](images/output1.png)

### ✅ Final JSON File
![Clean JSON Output](images/output2.png)

## 5. Future Improvements

- Use Pandas pipeline for large files
- Add automatic currency detection
- Add logging and error handling
- Support Excel and other file formats
