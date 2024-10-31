  #Tools in Data Science --> Project - 1 -- GitHub Users in Sydney with 100+ Followers --

**Data Collection:** Using the GitHub API, we retrieved all users in Sydney with over 100 followers, along with up to 500 of each user’s most recent repositories.

**Interesting Finding:** We found that a surprising number of highly-followed GitHub users in Sydney are affiliated with startups and open-source projects, showing strong community engagement.

**Developer Recommendation:** To increase visibility, developers should consider open-sourcing more projects and engaging with the GitHub community.


**Project Overview**

This repository contains data about GitHub users in Sydney who have more than 100 followers and their public repositories. The data was collected using the GitHub API and organized into two main CSV files, users.csv and repositories.csv, along with the Python script used for data scraping.

**Files in this Repository**
1. users.csv: Contains details about GitHub users located in Sydney with 100+ followers, including fields such as username, company affiliation, bio, followers, and repository counts.

2. repositories.csv: Contains details about the public repositories of users in users.csv, including fields like repository name, creation date, star count, language, and license type.


**How Data Was Collected:**
The GitHub scraping process was handled using the GitHub API, focusing on users in Sydney with a follower count of over 100. Data retrieval involved iterating through users and fetching repository information for each user, subject to API rate limits. Company names were cleaned to remove extra spaces, @ symbols, and were converted to uppercase. The API’s rate limit was handled by automatically pausing when limits were reached.


**Users and Repositories CSV Schema**

**users.csv Columns:**
Each row in users.csv corresponds to a GitHub user and contains the following fields:

login: The GitHub user ID.
name: The full name of the user.
company: The user's company affiliation, cleaned up (uppercase, no leading @).
location: The user's location (expected to be Sydney).
email: User's email address, if available.
hireable: Whether the user is open to job offers (true/false).
bio: The user’s bio or personal description.
public_repos: Number of public repositories owned by the user.
followers: Number of followers the user has.
following: Number of users the user is following.
created_at: Date when the user created their GitHub account.

**repositories.csv Columns:**
Each row in repositories.csv represents a public repository associated with a user from users.csv. The fields include:

login: GitHub user ID (login) of the repository owner.
full_name: Full name of the repository.
created_at: Date when the repository was created.
stargazers_count: Number of stars received by the repository.
watchers_count: Number of watchers for the repository.
language: Primary programming language of the repository.
has_projects: Boolean indicating if projects are enabled for this repository.
has_wiki: Boolean indicating if a wiki is enabled for this repository.
license_name: License type for the repository (derived from license key if available).


Observations and Recommendations
Through analyzing this dataset, several insights emerged about GitHub users in Sydney and their projects:
1. Active Community Engagement: A notable portion of users are involved with startups or contribute regularly to open-source projects.
2. Language Preference: Most popular programming languages among repositories include JavaScript, Python, and TypeScript, reflecting a diverse but common stack.

Recommendations for Developers
To gain followers and community engagement:

Collaborate with Open Source: Developers should consider contributing to or initiating open-source projects to build their professional network and increase visibility.
Optimize Repository Setup: Ensuring that repositories have documentation, a clear license, and are set up for collaborative features (like wikis and projects) can attract more engagement.
This user.csv contains data about GitHub users based in Sydney with over 100 followers, as well as their repositories.

