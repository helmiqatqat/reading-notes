# Access Control (ACL)

## 5 steps to RBAC

**What is Role Based Access Control (RBAC) and why do we care?**

- RBAC is the idea of assigning system access to users based on their role within an organization.

**Describe a Role/Permission heirarchy that you might implement using RBAC.**

- Superadmin:
  - Permissions: This role has full access and control over all system resources and administrative functions. They can perform tasks such as user management, role assignment, and system configuration.

- Admin:

  - Permissions: Admins have administrative privileges within specific domains or departments. They can manage users, roles, and resources within their assigned domain. However, they do not have the same level of control as Superadmins.

- Manager:

  - Permissions: Managers have permissions to manage resources and users within their assigned teams or projects. They can perform tasks such as creating, modifying, or deleting resources, assigning roles to team members, and viewing team-specific data.

- User:

  - Permissions: Users have basic permissions necessary to perform their day-to-day tasks. They can access and interact with resources relevant to their roles and responsibilities. However, they do not have administrative privileges or the ability to modify system-wide settings.

**What approach might you take to implement RBAC?**

- Identify Roles: Begin by identifying the different roles within your system or organization. Roles should represent distinct job functions or responsibilities that users may have. For example, you might have roles such as Superadmin, Admin, Manager, and User.

- Define Permissions: Determine the specific permissions that are required for each role. Permissions should reflect the actions or operations that users can perform on system resources. For example, permissions could include read, write, create, delete, or execute actions.

- Assign Permissions to Roles: Assign the appropriate permissions to each role based on the requirements of the job function or responsibility associated with that role. This step establishes the relationship between roles and permissions. Ensure that each role has the necessary permissions to fulfill its duties without granting excessive access.

- Map Users to Roles: Map individual users to the appropriate roles based on their job function or responsibility. Users can be assigned to one or multiple roles, depending on their responsibilities within the organization.

- Implement Access Control: Implement access control mechanisms based on the assigned roles and associated permissions. This can be achieved through various means, such as access control lists (ACLs) or user/group permissions in an operating system, or by utilizing RBAC frameworks or libraries provided by programming languages or frameworks.

- Role Assignment and Management: Establish processes for managing role assignments and updates. This involves handling user role changes, such as promotions, transfers, or terminations. Ensure that access rights are adjusted accordingly based on these changes.

- Regular Auditing and Review: Perform regular audits and reviews of role assignments and permissions to ensure that they align with the evolving needs of the organization. This helps identify any discrepancies, outdated permissions, or potential security risks.

- Training and Documentation: Provide training and documentation to users, administrators, and other relevant personnel to ensure a clear understanding of RBAC policies, roles, and permissions. This helps users adhere to the access control model and facilitates proper usage and administration.

## wiki - RBAC

**If Authentication is “you are who you say you are,” what is Authorization?**

- Authorization is what authorities I am allowed to use.

**Name three primary rules defined for RBAC.**

- Three primary rules are defined for RBAC:

- Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.

- Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.

- Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.

**Describe RBAC to a non-technical friend.**

- You are an employee in a company, there are employees just like you and there are the team leaders, the project managers and the ceo. You do not have same permissions in the company as other higher level employees, but you have same permissions as the same level employees as you are, these kind of permissions are determined by the board of the company which in Web are called the admins, you as an employee are a user, and the higher level employees are what they have more permissions and authorizations from you.
