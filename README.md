## Design for a Flask Application: Website that Teaches Browsing

### HTML Files
- **index.html**: This file will:
  - Contain the main content of the website.
  - Provide an interface for users to interact with, such as a form for submitting search queries.

- **results.html**: This file will:
  - Display the results of the search query.
  - Provide options for browsing and filtering through the results.

### Routes

- **@app.route('/')**: This route will handle requests to the main page of the website. It will:
  - Render the **index.html** file.

- **@app.route('/search', methods=['POST'])**: This route will handle the search query submitted by the user. It will:
  - Retrieve the search query from the form in **index.html**.
  - Perform the search and store the results in a variable.
  - Redirect the user to the **results.html** page with the search results.

- **@app.route('/browse')**: This route will handle requests to browse the search results. It will:
  - Display a list of all the search results.
  - Allow users to filter the results by various criteria, such as relevance, date, or popularity.

- **@app.route('/filter')**: This route will handle requests to filter the search results. It will:
  - Retrieve the filtering criteria from the user.
  - Filter the search results according to the specified criteria.
  - Display the filtered results to the user.