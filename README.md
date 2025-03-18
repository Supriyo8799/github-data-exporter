# GitHub Data Exporter

A tool to export GitHub user's followers, following, repositories, starred repositories, gists, and starred gists as CSV files in a ZIP archive.

## Features

- **Export Followers**: Get a list of followers of a GitHub user.
- **Export Following**: Export a list of users that the GitHub user is following.
- **Export Repositories**: List all repositories, including both public and private repositories of the user.
- **Export Starred Repositories**: Fetch and export a list of repositories a user has starred on GitHub.
- **Export Gists**: Export a list of public and private gists associated with the user.
- **Export Starred Gists**: Export a list of starred gists associated with the user.

> **Note**: This tool only lists the **followers**, **following**, **repositories**, **starred repositories**, **gists**, and **starred gists** of a GitHub user. It does not include other data such as project details or code from repositories.

## How to Use

1. Enter your **GitHub username** and **GitHub Personal Access Token**.
2. Click **Get Data** to fetch the GitHub data (followers, following, repositories, starred repositories, gists, and starred gists).
3. After data is fetched, a **Download CSV Files** button will appear.
4. Click **Download CSV Files** to download a ZIP archive containing:
   - `github_followers_<username>.csv` (Followers list)
   - `github_following_<username>.csv` (Following list)
   - `github_repositories_<username>.csv` (Repositories list)
   - `github_starredrepositories_<username>.csv` (Starred repositories)
   - `github_gists_<username>.csv` (Gists list)
   - `github_starredgists_<username>.csv` (Starred gists list)

## How to Get a GitHub Personal Access Token

1. Go to [GitHub Personal Access Tokens](https://github.com/settings/tokens).
2. Click **Generate New Token**.
3. Select the following **scopes**:
   - **`repo`**: Grants full control over private and public repositories, including reading, writing, and managing them. This is required to access the repositories (both public and private).
   - **`gist`**: Grants access to your public and private gists. This scope is necessary to export gists data.
   - **`user`**: Grants access to public user data, including followers and following. This scope is required to get the followers and following data.
4. Click **Generate Token** and copy it.
5. Paste the token into the input field in the app.

> **Warning**: Please ensure that you do not share your **GitHub Personal Access Token** with others. It provides access to sensitive data and should be kept private. Treat it like a password.

## Tools Used

- **HTML**: The core structure of the application is built using HTML.
- **CSS**: Used for styling and layout of the exporter.
- **JavaScript**: Used for the interactivity and functionality of the exporter.
- **JSZip**: A library to generate the ZIP archive of CSV files for download.
- **GitHub API**: Used to fetch data from GitHub.

## License

This project is licensed under the **No License**.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/feature-name`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/feature-name`).
5. Create a new pull request.

## Contact

For any issues or feature requests, please open an issue in the repository.
