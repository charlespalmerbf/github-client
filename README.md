GitHub Client Flutter App
=========================

The GitHub Client Flutter App is a sample Flutter app that demonstrates how to authenticate with the GitHub API using OAuth and fetch data from the API.

Installation
------------

To use the GitHub Client Flutter App, clone the repository and run the following command in the root directory of the project:

bashCopy code

`flutter run`

This will launch the app on your default device or emulator.

Usage
-----

The app allows you to log in to your GitHub account using OAuth authentication and view a summary of your GitHub activity.

To log in, tap the "Log in with GitHub" button on the home screen. This will redirect you to the GitHub login page where you can enter your GitHub credentials and authorize the app.

After logging in, you will see a summary of your GitHub activity, including your repositories, pull requests, and issues.

Implementation
--------------

The app is implemented using the following components:

-   `MyApp`: The main app widget that sets the app title and theme.
-   `MyHomePage`: The home screen widget that displays the app title and the `GitHubSummary` widget.
-   `GitHubSummary`: A widget that fetches data from the GitHub API using the `github` package and displays a summary of the user's GitHub activity.
-   `GithubLoginWidget`: A widget that handles the OAuth authentication flow and provides an `http.Client` object for making authenticated requests to the GitHub API.
-   `github_oauth_credentials.dart`: A file that contains the client ID, client secret, and scopes for the GitHub OAuth app.

The `WindowToFront` plugin is used to bring the app window to the front after the OAuth redirect.
