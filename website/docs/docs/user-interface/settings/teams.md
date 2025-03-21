---
title: Teams
---

Our Team Management feature allows you to manage the following capabilities:

* Allocate users and system accounts to teams
* Allocate applications to teams
* Assign team administrators
* Allocate environments to teams

_NOTE: Editing of teams is restricted to users with the `team:manage:*` permission (Administrators) or who have been assigned as Team Administrators by an existing user with the team manage permission._

![Teams Management Screen](/ui/clarity/settings-teams.png)

**A new Team** will allow you to create a new team and assign applications and environments to that team.

**Deleting a team** allows you to unlink all users, applications and environments from a team and remove it. Deleting the team will also disassociate any secrets and webhooks that were associated with the team. The secrets and webhooks that were disassociated will then be editable only by users with the `secret:manage:*` and `webhook:manage:*` permissions respectively (eg Administrators).

**Editing a team** allows you to change the name and applications of an existing team, assign Team Administrators and assign environments.

Clicking the team's name will take you to the selected team's screen.

## The "Default" team

The `contract_data:manage:team` permission that comes with the `User` role allows users to manage contract-related data (for example, publish pacts and verification results) for applications assigned to their teams. To help you get started with teams quickly, every new PactFlow account is set up with a special, system defined "Default" team. All new users and applications are automatically added to this team on creation.

The default team can be deleted once your own user defined teams have been created. From then on, users and applications will need to be assigned to teams explicitly through the UI. To ensure that your users can continue to manage their applications, you should create your own teams with the appropriate users and applications assigned before deleting the default team.

## Editing or Creating a team

![Edit Team](/ui/clarity/settings-teams-create.png)

With the team applications, you can search for applications and add them to the team. This allows the team users to be able to filter the main dashboard by those applications.

Lastly, environments can be allocated to the team here.

## Managing users in a team

![Edit Team Users](/ui/clarity/settings-teams-members.png)

You can search for users by name to add to the team. Users may also be removed from the team

Team Administrators can also be assigned or unassigned on this screen using the "Add" or "Remove" role option. Team Administrators can assign users and applications to a team, and update its name.

## Allocating System Accounts to a team

You can add and remove System Account users from a team from this screen.

![Edit Team System Accounts](/ui/clarity/settings-teams-system.png)
