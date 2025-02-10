# README

## Overview
This script fetches the number of Taiwan High-Speed Rail (THSR) trains traveling from Banqiao (\u677f\u6a4b) to Changhua (\u5f70\u5316) at 12:00 PM on a specified date using an HTTP POST request. It extracts and displays train schedule details such as train number, departure time, and arrival time.

## Prerequisites
- Python 3.x
- Jupyter Notebook (recommended)
- Required Python libraries:
  - `requests`
  - `BeautifulSoup4`
  - `json`

## Installation
Install the required libraries using pip:
```bash
pip install requests beautifulsoup4
```

## How to Use
1. Open Jupyter Notebook.
2. Copy and paste the script into a new notebook cell.
3. Update the `OutWardSearchDate` parameter in `payload` to the current date.
4. Run the script to retrieve train schedule information.

## Code Explanation
1. **Define Parameters:**
   - The payload dictionary contains search parameters, including departure station (`BanQiao`), arrival station (`ZhangHua`), date, and time.
2. **Send POST Request:**
   - The request is sent to `https://www.thsrc.com.tw/TimeTable/Search` with the payload and headers.
3. **Process Response:**
   - The response is parsed as JSON.
   - The script extracts train schedule data from the JSON and prints train details.

## Example Output
```plaintext
Train number: 1234, Departure time: 12:10, Destination time: 13:00
Train number: 5678, Departure time: 12:30, Destination time: 13:20
```

## Notes
- Ensure that the API endpoint is accessible.
- If the response format changes, the script may need adjustments.
- The request includes a user-agent header to mimic a browser request.

## License
This script is open-source and free to use.

