# TDS_project_1

# Boston GitHub User Analysis

* This project analyzes public GitHub data of users located in Boston with over 100 followers to identify trends and insights.
* The surprising analysis result was that language preference was not strongly tied to the year the user joined GitHub.
* Based on this analysis, Boston-based developers should consider updating their user bio regularly.


## Data Scraping

The data was scraped using the GitHub API. First, users located in Boston with more than 100 followers were identified using the Search API (`/search/users`). Then, for each user, their profile information was obtained (`/users/{username}`), and information about their first 500 public repositories was retrieved (`/users/{username}/repos`). The collected data was saved into two CSV files: `users.csv` (for user profiles) and `repositories.csv` (for repositories).



## Most Interesting Fact

While there were various findings, the observation that language preference is not strongly related to when a user joined GitHub was surprising. Intuitively, one might expect newer developers to gravitate toward more recently popular languages. However, the analysis revealed a diverse language landscape among users of different registration years. This suggests that individual choices and project needs strongly influence language adoption.



## Actionable Recommendation

The analysis showed a positive correlation between a developer's number of followers and the length of their bio in the GitHub profile. Therefore, a recommended action for developers aiming to increase their visibility and network within the Boston developer community is to create a well-written and informative bio. A detailed bio offers valuable insights into a developer's skills and interests, thereby attracting more followers and potential collaborators.
