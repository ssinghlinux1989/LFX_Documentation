# FAQs

### What types of access levels is CM  supporting?

CM is supporting 3 access levels to accommodate different roles and responsibilities within a community:

1. **Admin Access**: Full control over all projects, including the ability to manage settings, add/edit integrations, and edit contributors for all projects. Admins can also merge contributors and organizations in CM.
2. **CM Manager Access**: Ability to manage settings, add/edit integrations, and edit contributors for one or a limited number of projects. This role includes "read-only" permissions to view and explore contributors, organizations, and activity/contribution data for all projects. These users cannot merge contributors and organizations.
3. **Viewer Access**: Allows users to view contributor, organization, and activity/contribution data with "read-only" permissions for all projects.

### How is access control working for CM?

CM uses the same SSO system as other LFX products. A valid LF Account grants access to CM and access to a project in PCC automatically gives access to the same project in CM. This integration ensures a seamless user experience across LFX platforms.

### I want to give access to CM to my peers, what is the process to give access?

Contact the Support team and specify which project your peers need access to, along with their email and LF Account.

### Which permissions do I need to onboard the data source in CM?

To onboard a data source into CM, you need CM Manager Access within CM for managing the onboarding process, along with admin-level permissions for the data source you're integrating. For example, GitHub Onboarding requires Admin access to your GitHub organization because the onboarding process involves installing the CM GitHub application, which is essential for CM to collect data from GitHub.

### **What steps should I take if I don't have access to necessary tools like LinkedIn, GitHub, Slack, etc., for onboarding data**?

If you lack access to a required tool or platform for integration:

1. Find someone who has the necessary access and request that they either give you admin rights or share their login credentials with you.
2. Alternatively, you can reach out to the CM Support team and ask for temporary access for the person who has the needed access. This will enable them to log in to CM and set up the integration.

### **What should I do if I can't view or edit integrations for my projects when I log in**?

If you're experiencing issues with project permissions, such as not being able to see or edit integrations, contact the Support team for assistance.

### **What should I do if some sub-projects of my project or foundation are missing and not listed in CM**?

In case some sub-projects do not appearing in CM, reach out to the Onboarding team for support. They can assist in adding these missing projects or sub-projects to CM.

### **Why am I able to see data for all projects, not just my own**?

In CM, if you have "edit" access to your project, you can modify integrations for that particular project. However, for all other projects, you will have "viewer" access, which is limited to read-only and does not permit any modifications.

### What is the process if a project is created in PCC but not in CM?

If a project is present in PCC but does not automatically appear in CM, you should contact the onboarding team for assistance. They can facilitate adding the missing project to CM. This approach is applicable if a project is no longer relevant, needs to be hidden, or has been moved under a different project.

#### Data-Related Questions

### How long does it take for data to show up in CM?

The time it takes for data to appear in CM varies depending on the size of the projects and the type of integration.

* **Small Projects**: Data typically appears within a couple of hours.
* **Medium Projects**: Data visibility ranges from a few hours to a day.
* **Large Projects**: It can take a couple of days for data to be visible.
* **X-Large Projects**: Data from very large projects, such as GitHub repositories with tens of thousands of commits and PRs, may take a few days to a few weeks to show up.

### Why may the GitHub and Git data in CM be different compared to GitHub itself?

There are several reasons for differences between the data in CM and GitHub itself, including:

1. **Bot Account Exclusion**: CM does not collect data from bot accounts or contributions made by these accounts. In some cases, bot activities can account for as much as 50% of the total activities in a GitHub repository.
2. **Data Delay**: It is typical for CM to experience a delay in data collection. This delay can range from a few hours to a few days.

### **What action should I take if data isn't showing up in CM even after waiting 24 hours**?

If data still isn't appearing after 24 hours after onboarding or enabling new integration, reach out to the Onboarding team for assistance.

### **How do we determine the organization's history and other contributors' details, such as email, location, experience, etc.**?

Contributors' details are gathered from the information they provide on platforms like GitHub, Twitter, Slack, etc., and from their LinkedIn profiles.

### How do we get the contributor's LinkedIn profile?

An enrichment service is used to gather information about contributors' LinkedIn profiles and work history using their email and/or GitHub usernames.

### **What if GitHub or Gerrit data shows up in CM but does not show up in Insights V3**?

To resolve this, ensure that Git integration is enabled for all repositories added in the GitHub or Gerrit integration. Data will not appear in Insights until this Git integration is enabled. It's important to note that if a repository is not added to Git, Insights will not display data for it, regardless of whether GitHub integration is enabled and synced. To improve this process, there is a plan to introduce a feature that automatically populates Git integration based on the GitHub integration settings. If you are uncertain about the integration status, it is advisable to enable GitHub integration and seek assistance from the Onboarding Team.

### What should I do if contributors don’t have details like work history, location, experience, etc?

An enrichment service regularly updates each contributor shortly after they are added to CM and every few months thereafter. Some contributors may not be found in the enrichment databases and therefore will not be enriched.

### What should I do if the collected Contributor and Organization data for the project in CM are incorrect?

Check if integrations for your projects are set up correctly. If you do not have access to see and manage integrations, contact the Onboarding Team. Check if you have set the correct filter options. For example, you may be looking at data for the entire Foundation instead of a single project and may need to add a Project Filter. If the data is still incorrect, contact the Onboarding team.

### Do organizations and contributors get enriched with additional information after being added to CM?

Yes, after organizations and contributors are added to CM, they undergo enrichment through a dedicated service. This service enhances their profiles with additional details such as work history, location, organization logos, descriptions, and more.

### What if the contributor’s or organization’s data are not correct after they are enriched?

If you find inaccuracies in the enriched data for contributors or organizations, you have the option to manually edit and update this information. These manual updates will not be overridden by subsequent enrichment processes.

### **Why are there duplicate organizations in CM**?

Duplicates in organizations often occur due to varying information sources, such as LinkedIn or inputs from contributors, leading to slight differences in organization names. CM team is proactively working on merging these duplicates through automatic and manual processes. However, some duplicates might still exist. Efforts are underway to develop a feature that will allow users to merge these duplicate organizations themselves.

### **What causes duplicate contributors to appear in CM**?

In CM, contributors might have accounts on different platforms like GitHub, Git, Twitter, Slack, etc., known as “Identities.” Sometimes, a contributor uses the same name on multiple platforms, causing duplicates in CM. To solve this, CM uses an auto-merge feature to combine these identities.&#x20;

We also manually merge identities, especially for top contributors or when requested. However, you might still see duplicate contributors in CM. We’re developing a “merge” feature that will let users merge contributors, helping to remove these duplicates.

### **How do Git and GitHub identities differ in CM**?

In CM, a GitHub identity encompasses a user's GitHub profile, including their name, GitHub ID, logo, and public details like company information. Conversely, a Git identity is more basic, typically consisting of just the name and email address as they appear in the Git log.

### **What distinguishes default affiliation from manual affiliation in CM**?

Default auto-affiliation, derived from sources like LinkedIn or GitHub identities, represents a user's general work history without specific start and end dates. Manual affiliation, or project-level affiliation, is an alternative used to specifically link a developer's activities to a particular project, ideal for correcting or fine-tuning affiliations.

### How do we validate data in CM?

Our testing includes both automated and manual methods. We use an internal QA automation framework for high-level validation of data from most onboarded repositories, primarily for platforms like GitHub. For detailed scrutiny, such as with groups.io, we conduct manual testing to ensure the accuracy and completeness of the data integration.

#### Merge Suggestion Feature

### What is the logic used for the merge suggestion feature? (Note: Merge feature is currently unavailable)

Merge suggestions for organizations and contributors are based on their similarities. For organizations, suggestions consider similarities in names and domains. For contributors, the suggestions are based on names and email addresses.

### **Why is the feature for merging organizations and contributors currently disabled in CM**?

To ensure the integrity and accuracy of our data management, we have decided to restrict the task of organization and contributor merges exclusively to our internal team. This decision is due to the irreversible nature of these merges – currently, we lack a straightforward method to cleanly reverse or unmerge them once completed. We believe this approach is essential to maintain the quality and reliability of our organizational data.

### What happens when I merge records? (Note: Merge feature is currently unavailable)

Merging two contributors or organizations involves choosing a primary profile. For contributors, some details like the name and profile picture are taken from the primary profile, while others like work history, emails, and activities are combined from both profiles. For organizations, certain information like the logo, domain, and description are from the primary organization, while other details are merged. Note that organization merges are irreversible, and contributor merges are partially reversible but require manual intervention. For manual individual contributor unmerges, requests can be made in CM.

### What are our plans for the unmerged feature and audit log?

An automatic "unmerge" feature for contributors and organizations is planned, allowing users to reverse previous merges. We are also developing an audit log to track individual merges.

#### Other Questions

### **What is the function of the onboarding team in CM, and how can I contact them**?

The Onboarding team plays a crucial role in helping projects and maintainers integrate their work with the CM tool. They can be reached for support via the Slack channel 'lfx-insights-onboarding-support' or through a Jira ticket.



