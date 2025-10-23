# Managing Teams (for Administrators)

The page includes basic steps and links to official documentation for managing teams, roles, and organization wide member permissions. While not comprehensive, enough information is provided to adequately get started in managing members and their corresponding teams.

> All steps shown below are starting from the main Organization GitHub Page.

## Setting Orginization-wide Base Member Permissions
Anyone who becomes a member automatically inherits some permission to the organization, even before being added to a Team. This is why it is important to set base permissions that you are fine with all members inheriting. To do so,<br>
`Settings > Member privileges > [set base permission to either "read" or "None"]`

You can also step through the `Member privilege` page and fine-tune the other base settings to your liking.

## Assigning different permissions to specific Teams
To assign more permissive permissions to specific teams (that members will then inherit):<br>
`Settings > Organization roles > Role assignments > New role assignment > [select a permission level and search for a team (or member)] > follow remaining prompts`

To manage existing roles, simply use the same page. To give higher privileges for a specific repository to a particular Team: <br>
`Teams > [select team] > Repositories > Add repository`

## Moving Members Between Teams

While GitHub does not offer a simple way to "drag-drop" members between Teams, it does make it easy to remove and add members. In this way members can be organized into Teams. It is by being part of a Team that any particular member inherits read/write/maintain/admin permissions. Thus, it is crucial that teams are properly managed for decent project security and member cohesion.

To **add a member**:<br>
`Teams > [click on a team] > Add a member > [search for name] > follow remaining prompts`

To **remove a member**:<br>
`Teams > [click on a team] > [click on checkbox next to the member's profile] > Remove from team [in the dropdown above the checkboxes]`

## Making trusted members full Owners

Admin permissions, although permissive, are not as permissive as the privileges gained by being a full-fledged owner. To add a member as an owner with full control of the Organizations GitHub Account:<br>
`People > [select member] > [dropdown under profile] > set as "Owner"`

This, of course, can be reversed at anytime.

## Additional GitHub Documentation for Administrators

- <https://docs.github.com/en/organizations>
- <https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/about-organizations>
