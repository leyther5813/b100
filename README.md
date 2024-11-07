## Project Overview

- **Data Scraping Method**: Used the GitHub API to fetch user data and repository information for users in Bangalore with over 100 followers.
- **Interesting Finding**: A surprising insight was the high concentration of popular repositories in Python, indicating its strong developer community presence in Bangalore.
- **Recommendation for Developers**: To increase visibility, developers in Bangalore might consider adding project descriptions and using popular tags to improve discoverability.

---

### Files

This project contains the following files:
- `users.csv`: Contains detailed information about each user in Bangalore with over 100 followers, including user ID, name, company, and other relevant details.
- `repositories.csv`: Lists up to 500 recent repositories for each user, with information on repository name, creation date, language, and star count.
- `README.md`: This document.

---

### Data Collection Process

1. **Fetching Users**: Used GitHub's Search Users API to retrieve users in Bangalore with over 100 followers. For each user, additional details were fetched to populate the `users.csv` file.
2. **Fetching Repositories**: For each user, retrieved up to 500 of their most recently pushed repositories, capturing details like repository name, star count, and language to populate `repositories.csv`.
3. **Data Cleaning**: Company names were standardized by trimming whitespace, removing the initial '@' symbol (if present), and converting to uppercase.
