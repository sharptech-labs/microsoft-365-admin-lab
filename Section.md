<h2>Section 3 — Role Assignment &amp; Conditional Access Configuration</h2>

<h3>Assigning Administrator Roles in Entra ID</h3>

<p>
  I assigned myself the Global Administrator role to ensure full access while configuring the tenant.
  I then assigned the IT Admins security group the User Administrator, Helpdesk Administrator, and Global Reader roles.
  This created a layered permission model where admin‑level accounts receive elevated capabilities without granting full control to every member.
</p>

<img src="https://imgur.com/omLvm0g.png" width="800">
<img src="https://imgur.com/UPrPkAB.png" width="800">
<img src="https://imgur.com/WxVxRTA.png" width="800">
<img src="https://imgur.com/XeG34lM.png" width="800">

<p><strong>Purpose:</strong> Establishes a secure RBAC structure by granting the minimum required admin privileges to the appropriate group while maintaining a dedicated Global Administrator for tenant‑wide control.</p>

<hr>

<h3>Testing IT Admin Permissions</h3>

<img src="https://imgur.com/zFSr5yV.png" width="800">

<p>
  After assigning roles to the IT Admins group, I signed in using an account that was a member of that group to verify the permissions were applied correctly.
  I successfully reset another user’s password, confirming that the delegated admin roles were functioning as intended.
</p>

<img src="https://imgur.com/2y5u9Tj.png" width="800">
<img src="https://imgur.com/3vKCL3V.png" width="800">

<p><strong>Purpose:</strong> Validates that group‑based role assignments are working and confirms that delegated admin permissions are correctly applied to members of the IT Admins group.</p>

<hr>

<h3>Creating the “Require MFA – Standard Users” Conditional Access Policy</h3>

<img src="https://imgur.com/LHiDyRW.png" width="800">

<p>
  I created a Conditional Access policy that enforces MFA for all standard users.
  The policy includes the Standard Users security group and excludes the IT Admins group to prevent locking out privileged accounts during configuration.
  The policy targets all cloud apps and requires MFA as the access control.
</p>

<img src="https://imgur.com/eYQTCDW.png" width="800">
<img src="https://imgur.com/7lLve15.png" width="800">
<img src="https://imgur.com/oYHHRps.png" width="800">
<img src="https://imgur.com/mPqGLPv.png" width="800">
<img src="https://imgur.com/Jv3qdqn.png" width="800">
<img src="https://imgur.com/hBQOfay.png" width="800">
<img src="https://imgur.com/BhzNeg0.png" width="800">

<p><strong>Purpose:</strong> Enforces strong authentication for regular users while protecting admin accounts from misconfiguration during early tenant setup.</p>

<hr>

<h3>Disabling Security Defaults</h3>

<p>
  Before enabling my Conditional Access policies, I disabled Security Defaults in Entra ID.
  Security Defaults must be turned off because they enforce their own baseline MFA requirements, which conflict with custom Conditional Access policies.
</p>

<img src="https://imgur.com/zixRzOs.png" width="800">
<img src="https://imgur.com/GBP4hpH.png" width="800">
<img src="https://imgur.com/RjyKUh2.png" width="800">

<p><strong>Purpose:</strong> Allows Conditional Access policies to take precedence by removing the built‑in Microsoft security baseline, ensuring that my custom MFA enforcement works as intended.</p>

<hr>

<h3>Creating the “Privileged Access – IT Admins” Conditional Access Policy</h3>

<p>
  I created a Conditional Access policy specifically for privileged accounts.
  This policy includes the IT Admins security group and excludes my personal Global Administrator account (Henry Meiners) as a break‑glass safeguard.
</p>

<img src="https://imgur.com/rR6L9Ql.png" width="800">
<img src="https://imgur.com/e5XReWK.png" width="800">

<h4>Key Security Controls Configured</h4>

<p><strong>Require device to be marked as compliant</strong> — ensuring that admin access is only allowed from Intune‑managed, compliant devices.</p>
<img src="https://imgur.com/Ts6AAgM.png" width="800">

<p><strong>Targeted only essential admin resources</strong> — including Microsoft Admin Portals and Azure Resource Manager, instead of “All cloud apps,” to avoid accidental lockouts and maintain a controlled, least‑privilege enforcement scope.</p>
<img src="https://imgur.com/BU9YCSL.png" width="800">

<p>
  I configured the Client Apps condition to apply the policy to both browser access and modern authentication clients,
  ensuring that administrative sign‑ins are protected across web and desktop/mobile applications while excluding legacy authentication clients.
</p>

<img src="https://imgur.com/a6YhvUs.png" width="800">

<p><strong>Purpose:</strong> Enforces stronger security requirements for administrative access by combining MFA, device compliance, and scoped resource targeting, while preserving guaranteed access through a break‑glass exclusion.</p>

<img src="https://imgur.com/CEJsbXZ.png" width="800">
