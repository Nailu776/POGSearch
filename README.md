# POGSearch

POGSearch began as a focused solution for indexing repositories from private GitLab instances, enabling comprehensive text searches across multiple repositories, branches, and commits. This approach allows users to find specific code snippets with a single query, eliminating the need to manually search each project. As the project has evolved, it has expanded to indexing any Git repository, with an eye towards becoming a versatile search stack for various data types in the future.

## Features and Tech Stack

### Current Capabilities:

- **Keycloak Authentication**: Ensures secure access, requiring successful login for user participation.
- **Vue.js Frontend**: A minimalist interface offering robust search functionalities and administrative tools.
  - **Admin Tools**:
    - Create roles with designated index patterns to control user access levels to specific data sets.
    - Add users and assign roles for controlled access.
    - Import repositories using public repository links.
  - **Researcher Tools**:
    - Conduct full-text searches with customized index patterns and queries.
    - Direct links to files within search results for quick access.
- **Docker Integration**: The entire system is encapsulated within a Docker Compose stack for seamless deployment and scalability.
- **Java Spring Boot API**: Facilitates backend operations, enhancing user interaction and data management.
- **OpenSearch**: Powers the search engine, offering scalable and effective search capabilities across vast datasets.

### Planned Enhancements:

- **Search Result View Format Enhancements**: Improving the presentation and accessibility of search results for a better user experience.
- **Commit Indexing**: Expand search functionalities to include comprehensive indexing of commits.
- **Bulk Import**: Admins can index multiple repositories or commits at once using a GitLab instance URL or a GitLab group URL along with an access token.
- **Selective Updates**: Intelligent updating of indexes based on modifications and new commits, avoiding full reindexing.
- **Auto Indexing**: GitLab integration for automatic indexing in response to changes in repositories.
- **User-Driven Data Configuration**: In the future, POGSearch may evolve into a platform where users can easily submit their data, configure access roles, and publish searchable content, thereby broadening its scope and utility.
- **Highly Optimized Multithreaded Data Processing Architecture**: Leveraging high-performance programming languages to enhance backend efficiency and scalability.

# Gallery
![login](https://github.com/Nailu776/POGSearch/assets/85428822/96b9f2f3-b858-4f8c-8503-1eff368b33e9)
![admin-panel](https://github.com/Nailu776/POGSearch/assets/85428822/c439033d-603d-4412-af1f-70663e455e3e)
Dev-Preview:
![search-dev-preview](https://github.com/Nailu776/POGSearch/assets/85428822/0fb93ddb-87a7-40a9-88a9-466f07138538)

