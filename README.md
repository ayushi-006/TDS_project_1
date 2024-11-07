# TDS_project_1

# Boston GitHub User Analysis

* This project analyzes public GitHub data of users located in Boston with over 100 followers to identify trends and insights.
* The surprising analysis result was that language preference was not strongly tied to the year the user joined GitHub.
* Based on this analysis, Boston-based developers should consider updating their user bio regularly.


## Data Scraping

The data was scraped using the GitHub API. First, users located in Boston with more than 100 followers were identified using the Search API (`/search/users`). Then, for each user, their profile information was obtained , and information about their first 500 public repositories was retrieved (`/users/{username}/repos`). The collected data was saved into two CSV files: `users.csv` (for user profiles) and `repositories.csv` (for repositories).



## Most Interesting Fact

### Repositories

* stargazers_count is highly overall correlated with watchers_count	<br>
* watchers_count is highly overall correlated with stargazers_count	 <br>
* has_projects is highly imbalanced (85.1%)	 <br>
* license_name is highly imbalanced (50.7%) <br>
* language has 10198 (24.0%) missing values	<br>
* license_name has 20173 (47.5%) missing values<br>
* stargazers_count is highly skewed (γ1 = 55.6457688)	<br>
* watchers_count is highly skewed (γ1 = 55.6457688)	<br>
* full_name has unique values	<br>
* stargazers_count has 26506 (62.4%) zeros <br>
* watchers_count has 26506 (62.4%) zeros <br>

![image](https://github.com/user-attachments/assets/887361a3-6710-4522-a1a4-b5a197c76b6b)


### Users

* company has 165 (35.2%) missing values	 <br>
* email has 233 (49.7%) missing values <br>
* bio has 154 (32.8%) missing values <br>
* login has unique values	 <br>
* created_at has unique values	 <br>
* following has 87 (18.6%)  <br>

![image](https://github.com/user-attachments/assets/8fcd807d-a203-491f-ae6d-5b443fa631e8)


## Actionable Recommendation

The analysis showed a positive correlation between a developer's number of followers and the length of their bio in the GitHub profile. Therefore, a recommended action for developers aiming to increase their visibility and network within the Boston developer community is to create a well-written and informative bio. A detailed bio offers valuable insights into a developer's skills and interests, thereby attracting more followers and potential collaborators.


The code for analysis and Scrapping are in Analysis.ipynb and Scrapping,ipynb


