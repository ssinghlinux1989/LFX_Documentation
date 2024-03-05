# Data Affiliation

Affiliation is a close association or connection to an organization, company, and so on. An example of affiliation is being a contributor to a community organization. Or, a contributor could belong to two or more companies that are related through common ownership but are treated as one. In this case, a single contributor might have multiple identities such as two different company emails. Data affiliation connects or associates these identities.

Insights uses _Identities and Affiliations_ to handle data affiliations as follows:

## Data Sources and Tools <a href="#dataaffiliation-datasourcesandtools" id="dataaffiliation-datasourcesandtools"></a>

Open source projects rely on a variety of data sources and tools to support and coordinate development activities, for example:

* Git repositories, such as Gerrit or GitHub projects
* Issue trackers such as Jira, GitHub Issues or Bugzilla
* Messaging tools such as Slack, Groups.io or mailing lists
* Build tools such as Jenkins

Project contributors can access the tools using different identities, for example: email, username. In Insights, each contributor has a _profile_. A profile has personal details and can include multiple identities and organization affiliations.

## Identities <a href="#dataaffiliation-identities" id="dataaffiliation-identities"></a>

An identity can be a combination of email address, full name, or username. Examples of identities are "commit signatures" (that is, full names and email addresses) of committers and authors in Git repositories. However, the identities used by the same profile (contributor) may diﬀer across the tools used in the project. A project profile might use more than one identity for the same tool (for example, in version control systems and mailing lists). In addition, an identity can be shared by project profiles, such as during pair programming (that is, the same email address for both profiles).

Insights manages identities across sources allowing identities to be affiliated, for example, a company and organization affiliation. In a database, identity and affiliation data is stored across domains. INSIGHTS evaluates individual contributions to open source projects by tracking the unique identities of profiles and their related information such as country and organization. Projects then produce meaningful statistics about their communities, because individual contributions are not underestimated.

## Analysis <a href="#dataaffiliation-analysis" id="dataaffiliation-analysis"></a>

An analysis of the enriched information (identities, affiliation, bot status, and so on) allows for a correct count of developers and others in software development. INSIGHTS retrieves the data, stores it in databases, analyzes it, and produces dashboards for visualizing the resulting information. The results let you measure any project as a whole using aggregated data of more than one type.
