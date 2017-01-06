# xAPI.NET: Setup

THIS DOCUMENT IS CURRENTLY IN DRAFT.

## Requirements

- Server environment support for the ASP.NET Core framework.
	- [GearHost](https://www.gearhost.com?refcode=reqfh32qhn5p) is one such provider. They also allow you to host 100 developer sites (with databases) for free. This link will provide you $10 to start.
- Microsoft SQL Server is our database of choice for this project.
	- Entity Framework Core has a [set of providers for other types of databases](https://docs.microsoft.com/en-us/ef/core/providers/). It should not be a heavy lift to make this project work with one of the providers in this list.
- HTTPS is highly recommended but not technically required.
	- Please see [Let's Encrypt for a free SSL certificate](https://letsencrypt.org/).
