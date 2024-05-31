# Location Taker

This project captures the user's geolocation and device information and then sends it to the specified Google Sheets script URL.

## Usage Instructions

### Spreadsheet URL Preparation

1. Visit the following repository to get the Spreadsheet URL:
   [Form to Google Sheets](https://github.com/jamiewilson/form-to-google-sheets)

2. Create a table like the following image, adjust it with the form coding used or as per your requirements:
![image](https://github.com/anggeryoga/location-take/assets/139601862/b1073a15-7c8e-4fac-9f31-7795d1339cda)

### How to Use

1. Clone the repository to your local computer:

    ```sh
    git clone https://github.com/anggeryoga/location-take.git
    ```

2. Open `index.html` in your web browser.

3. When the page loads, users will be prompted to allow location access. If users grant permission, the following steps will occur:
   - The user's geolocation (latitude and longitude) will be captured.
   - Device information such as the user agent string will be collected.

4. The captured data will then be automatically sent to the specified Google Sheets script URL.

### Important Notes

- Ensure that the browser supports geolocation. Most modern browsers support this feature, but some may require HTTPS for geolocation services to function.
- Users must grant permission to access their location. If permission is denied, location data will not be captured and an error message will be logged in the console.

### Troubleshooting

- If the location cannot be retrieved, make sure the location settings on the user's device are enabled.
- If the data is not sent to Google Sheets, recheck the script URL used and ensure the table in Google Sheets matches the data being sent.

---
