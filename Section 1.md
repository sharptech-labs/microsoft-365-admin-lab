<h2>Section 1 — User Lifecycle Management in Microsoft 365</h2>

<h3>Creating Users</h3>

<img src="https://imgur.com/xHM3xQb.png" width="800">

<p>
  I created new user accounts through the Microsoft 365 Admin Center. The process included entering basic identity information (name, username, and domain), confirming whether the user must reset their password at first sign‑in, selecting the initial password option, license assignment to ensure the account had access to required services immediately, and lastly the roles associated with that user.
</p>

<img src="https://imgur.com/oQBQq2k.png" width="800">
<img src="https://imgur.com/Q6S7Gck.png" width="800">
<img src="https://imgur.com/uHAG7Bz.png" width="800">
<img src="https://imgur.com/BKbdHfM.png" width="800">
<img src="https://imgur.com/mGKSRwp.png" width="800">
<img src="https://imgur.com/buiwCWf.png" width="800">

<p><strong>Purpose:</strong> Establishes the user’s cloud identity in Entra ID and prepares the account for authentication and service access.</p>

<hr>

<h3>Resetting Passwords</h3>

<img src="https://imgur.com/bv16FmI.png" width="800">

<p>
  I reset a user’s password from the page using the auto‑generated temporary password option and the “Require this user to change their password when they first sign in” option remained enabled to ensure the temporary password was only used once. After generating the password, the admin center displayed it in a confirmation window, allowing it to be copied and provided to the user through a secure communication method.
</p>

<img src="https://imgur.com/FIaExRC.png" width="800">
<img src="https://imgur.com/znLDpaO.png" width="800">

<p><strong>Purpose:</strong> Reflects a standard helpdesk workflow for restoring account access while maintaining secure password handling practices.</p>

<hr>

<h3>Blocking and Unblocking Sign‑In</h3>

<img src="https://imgur.com/n0RZBoE.png" width="800">

<p>
  I used the “Block sign‑in” to prevent a user from authenticating without deleting the account. This action immediately restricts access to all Microsoft 365 services. The sign‑in block was removed to restore normal access.
</p>

<img src="https://imgur.com/dESklfq.png" width="800">
<img src="https://imgur.com/f3dgyAd.png" width="800">
<img src="https://imgur.com/e81sSjs.png" width="800">
<img src="https://imgur.com/r4tttSy.png" width="800">
<img src="https://imgur.com/CfndSPb.png" width="800">

<p><strong>Purpose:</strong> Provides a fast, reversible method for containing compromised accounts or temporarily suspending access during HR or security events.</p>

<hr>

<h3>Deleting and Restoring Users</h3>

<img src="https://imgur.com/VZw3uBw.png" width="800">

<p>
  I deleted an account from the active user list to observe the soft‑delete behavior. Deleted accounts moved into the “Deleted users” section, where they remained recoverable for 30 days. Restoring the user reinstated their identity, mailbox, and associated data.
</p>

<img src="https://imgur.com/VQCjwP4.png" width="800">
<img src="https://imgur.com/ZWXTlAs.png" width="800">
<img src="https://imgur.com/wQySgDh.png" width="800">
<img src="https://imgur.com/wBhiD1X.png" width="800">
<img src="https://imgur.com/vBybbbu.png" width="800">

<p><strong>Purpose:</strong> Validates the user lifecycle process and demonstrates how Microsoft 365 protects organizations from accidental deletions or premature offboarding.</p>

<hr>

<h3>Assigning and Managing Licenses</h3>

<img src="https://imgur.com/t865f5r.png" width="800">

<p>
  I assigned a license from the user’s profile by selecting the appropriate Microsoft 365 SKU. The tenant‑wide license overview was reviewed to confirm total licenses, assigned licenses, and remaining availability.
</p>

<img src="https://imgur.com/nO4YHAE.png" width="800">
<img src="https://imgur.com/2HdyZYw.png" width="800">
<img src="https://imgur.com/ZJfxskf.png" width="800">
<img src="https://imgur.com/xdLR2Ic.png" width="800">
<img src="https://imgur.com/UHEemZe.png" width="800">

<p><strong>Purpose:</strong> Ensures users receive the correct services and helps maintain awareness of license consumption across the tenant.</p>

<hr>

<h3>Bulk User Creation via CSV</h3>

<img src="https://imgur.com/Rg0xML1.png" width="800">

<p>
  I created multiple users at once using the CSV import tool. I downloaded the Microsoft 365 template, populated it with user details, added licenses, and uploaded it for processing. The system validated the file and created all users listed in the CSV.
</p>

<img src="https://imgur.com/fjgt1L2.png" width="800">
<img src="https://imgur.com/9CQyhjZ.png" width="800">
<img src="https://imgur.com/s9ztzM9.png" width="800">
<img src="https://imgur.com/DV0ILHW.png" width="800">
<img src="https://imgur.com/5SZiwjx.png" width="800">

<p><strong>Purpose:</strong> Demonstrates scalable onboarding for larger groups and confirms the bulk provisioning workflow functions correctly.</p>
