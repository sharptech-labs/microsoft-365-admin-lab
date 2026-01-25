<h1>Microsoft 365 Administration &amp; Helpdesk Lab</h1>

<p>
  This repository documents my end-to-end Microsoft 365, Entra ID, Intune, Exchange, and Teams helpdesk environment.
  I built this lab to demonstrate real-world administration skills, including identity lifecycle management, RBAC,
  Conditional Access, Intune compliance, Teams collaboration structure, and Exchange configuration.
  Each section contains screenshots and documentation showing the exact steps I performed and the reasoning behind them.
</p>

<hr />

<h2> Section Overview</h2>

<h3>Section 1 — User Lifecycle Management in Microsoft 365</h3>
<p>
  I created new cloud user accounts, assigned licenses, reset passwords, and performed bulk user creation using CSV import.
</p>
<p><strong>Purpose:</strong> Demonstrates core identity lifecycle tasks and shows how Microsoft 365 handles onboarding, password resets, licensing, and bulk provisioning.</p>

<hr />

<h3>Section 2 — Security Group Management in Microsoft 365</h3>
<p>
  I created department-based security groups (HR, Sales, Finance, IT, Operations) and role-based groups (IT Admins, Standard Users),
  then assigned users to each group.
</p>
<p><strong>Purpose:</strong> Establishes a clean RBAC structure for policy targeting, permissions, and scalable identity management.</p>

<hr />

<h3>Section 3 — Role Assignment &amp; Conditional Access Configuration</h3>
<p>
  I assigned admin roles in Entra ID, tested delegated permissions, disabled Security Defaults, and created two Conditional Access policies:
</p>
<ul>
  <li><strong>Require MFA – Standard Users</strong></li>
  <li><strong>Privileged Access – IT Admins</strong> (with MFA, compliant device requirement, client app scoping, and targeted admin resources)</li>
</ul>
<p><strong>Purpose:</strong> Implements secure authentication and privileged access controls while maintaining a break-glass exclusion for safety.</p>

<hr />

<h3>Section 4 — Intune Compliance Policies &amp; Device Enrollment</h3>
<p>
  I created separate compliance policies for admin devices and standard devices, enrolled my local PC, resolved non-compliance issues,
  and confirmed successful compliance reporting.
</p>
<p><strong>Purpose:</strong> Demonstrates Intune device governance, troubleshooting, and role-based compliance baselines.</p>

<hr />

<h3>Section 5 — Microsoft Teams &amp; Jira Integration</h3>
<p>
  I created Microsoft 365 Groups and Teams for Sales, Operations, and Support. Inside the Support Team, I built a full helpdesk structure
  with channels, folders, OneNote notebooks, Jira Cloud app integrations, and SharePoint connections.
</p>
<p><strong>Purpose:</strong> Mirrors a real helpdesk environment with organized documentation, ticket visibility, escalation workflows, and integrated collaboration tools.</p>

<hr />

<h3>Section 6 — Shared Mailbox &amp; Distribution List Configuration</h3>
<p>
  I created a shared mailbox for the Support Team and configured delegation. I also created distribution lists for Tier 1 Support,
  Tier 2 Support, and All Users, adding the appropriate members.
</p>
<p><strong>Purpose:</strong> Centralizes support communication and enables efficient organization-wide and tier-based email distribution.</p>

<hr />

<h2> Skills Demonstrated</h2>
<ul>
  <li>Microsoft 365 user lifecycle management</li>
  <li>Entra ID identity and access administration</li>
  <li>Role-based access control (RBAC)</li>
  <li>Conditional Access policy design</li>
  <li>Intune device enrollment and compliance</li>
  <li>Teams collaboration structure and governance</li>
  <li>Jira Cloud integration with Teams</li>
  <li>Exchange shared mailbox and distribution list management</li>
  <li>Realistic helpdesk workflow design</li>
  <li>Documentation and screenshot-based process tracking</li>
</ul>

<hr />

<h2> About This Project</h2>
<p>
  This lab simulates a real organization’s IT environment, including:
</p>
<ul>
  <li>Departmental structure</li>
  <li>Support tiers</li>
  <li>Admin vs. standard user separation</li>
  <li>Device compliance enforcement</li>
  <li>Secure authentication</li>
  <li>Ticketing workflows</li>
  <li>Documentation management</li>
</ul>
<p>
  Each section contains screenshots and explanations showing exactly what I configured and why.
</p>
