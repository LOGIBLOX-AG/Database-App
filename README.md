# LOGIBLOX CRUD Example App

This is a simple example CRUD (Create, Read, Update, Delete) application for interacting with the LOGIBLOX Back-End API. It allows you to manage data points using a simple interface.

## Getting Started

To get started with the LOGIBLOX CRUD example app, follow these steps:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/logiblox-crud-app.git
   ```

2. **Navigate to the Project Directory:**

   ```bash
   cd logiblox-crud-app
   ```

3. **Upload data file**

    For this example we use the datafile `data/table.csv` which is included in this repo. Upload it to LOGIBLOX and and press the connector symbol to open up the API menu. 

    Make sure that you set the Lead ID column to the index, which uniquely identifies each row allowing row-specific operations such as update and delete.
   
   ![image](https://github.com/filipLBX/logiblox-crud-app/assets/149149449/bc037a28-9483-4a51-a880-9ce9cb4315a8)


5. **API key set-up:**
    
    First to create an API key for the datafile, go to the __Share API Configurations__ and then navigate to __Share API__ and add a new key.

   ![share_api](https://github.com/filipLBX/logiblox-crud-app/assets/149149449/32d5285a-9978-4070-92f3-ea8f1110d5fd)

    
    When the key is generated, we can add it to our react app using the following steps as guide:


   - Create a `.env.local` file in the project root.
   - Add the following environment variables to the `.env.local` file:
     - `REACT_APP_LOGIBLOX_API_URL` - Set this to the URL of your LOGIBLOX Datapoints API.
     - `REACT_APP_LOGIBLOX_API_KEY` - Set this to your API token.

   Example `.env.local` content:

   ```plaintext
   REACT_APP_LOGIBLOX_API_URL=https://your-logiblox-url.com/api/v0/datapoints/table
   REACT_APP_LOGIBLOX_API_KEY=your-api-key
   ```


7. **Install Dependencies:**

   ```bash
   npm install
   ```

8. **Start the Development Server:**

   ```bash
   npm start
   ```

9. **Access the Application:**

   Open a web browser and navigate to [http://localhost:3000](http://localhost:3000) to access the LOGIBLOX CRUD app.

## Usage

- The app allows you to create, read, update, and delete data points.
- Click the "Add" button to create a new data point.
- Click the "Update" button to modify a data point.
- Click the "Delete" button to remove a data point.

## Note

Ensure that you have the correct LOGIBLOX API URL and API token in your `.env.local` file. To make changes in the dotfile take effect, you have to restart npm.

Also, if you create additional tables, make sure that you enable your api key on each datafile you want to access in the __Share API Configuration__ menu.

## Learn More

For more information about LOGIBLOX, visit [LOGIBLOX](https://logiblox.com).

Happy managing your data points with LOGIBLOX CRUD API!

