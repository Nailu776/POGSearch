# POGSearch

## Video Preview
[![POGSearch Video Preview](https://github.com/Nailu776/POGSearch/assets/85428822/9f7a4414-246e-40fb-93ef-57500ff1ae9c)](https://drive.google.com/file/d/1Oun37QBJsSNsG4jkFyimEzPp0uTqweAJ/view?usp=sharing)

## Description
POGSearch began as a focused solution for indexing repositories from private GitLab instances, enabling comprehensive text searches across multiple repositories, branches, and commits. This approach allows users to find specific code snippets with a single query, eliminating the need to manually search each project. As the project has evolved, it has expanded to indexing any Git repository, with an eye towards becoming a versatile search stack for various data types in the future.

## Features and Tech Stack

### Current Capabilities:

- **Keycloak Authentication**: Ensures secure access, requiring successful login for user participation.
- **Vue.js Frontend**: A minimalist interface offering robust search functionalities and administrative tools.
  - **Admin Tools**:
    - Create roles with designated index patterns to control user access levels to specific data sets.
    - Add users and assign roles for controlled access.
    - Import repositories using repository links.
  - **Researcher Tools**:
    - Conduct full-text searches with customized index patterns and queries.
    - Direct links to files within search results for quick access.
- **Docker Integration**: The entire system is encapsulated within a Docker Compose stack for seamless deployment and scalability.
- **Java Spring Boot API**: Facilitates backend operations, enhancing user interaction and data management.
- **OpenSearch**: Powers the search engine, offering scalable and effective search capabilities across vast datasets.
- **Bulk Import**: Admins can index multiple repositories at once by providing an API URL, for example, to request projects within a group from GitLab, along with an access token if the group is private.
- **Scheduled Updates**: Admins can schedule updates for indices.

<details>
  <summary>Roadmap</summary>
  <br>
  <p>
    <strong>Current version:</strong> Alpha Tests
    <br>
    <strong>Todos:</strong>
    <ul>
      <li><strong>Beta version improvements:</strong>
        <ul>
          <li>Enable indexing of commit messages.</li>
          <li>Implement functionality to save search settings, such as index patterns and instant search preferences.</li>
          <li>Internationalization with i18n.</li>
          <li>Fine-tune indexes generation and query optimization.</li>
          <li>Enable selective updates (updating indexes based on modifications and new commits, avoiding full reindexing).</li>
          <li>Enable auto indexing (GitLab integration for automatic indexing in response to changes in repositories).</li>
        </ul>
      </li>
      <li><strong>Release version improvements:</strong>
        <ul>
          <li>Decompose project into modular components for enhanced reusability and extensibility.</li>
          <li><strong>User-Driven Data Configuration:</strong> Users can easily submit their data, configure access roles, and publish searchable content, thereby broadening its scope and utility.</li>
          <li><strong>Highly Optimized Multithreaded Data Processing Architecture:</strong> Leveraging high-performance programming languages to enhance backend efficiency and scalability.</li>
        </ul>
      </li>
    </ul>
  </p>
</details>

<details>
  <summary>Waitlist</summary>
  <br>
  <p>
    https://forms.gle/CZC8kgBQWBf7W7GQ7
  </p>
</details>
