<h2>Section 4 — Intune Compliance Policies &amp; Device Enrollment</h2>

<h3>Creating the “Windows Compliance – Admin Devices” Policy</h3>

<img src="https://imgur.com/SFB27aY.png" width="800">

<p>
  I created a Windows 10/11 compliance policy in Intune named “Windows Compliance – Admin Devices.”
  I assigned this policy to the IT Admins security group so that only administrative devices are held to these stricter requirements.
  The policy initially included settings such as TPM, BitLocker, and device encryption requirements.
</p>

<img src="https://imgur.com/fFK964l.png" width="800">
<img src="https://imgur.com/hZV1xD2.png" width="800">
<img src="https://imgur.com/nzbDn2U.png" width="800">
<img src="https://imgur.com/4JU2LdB.png" width="800">
<img src="https://imgur.com/CHCVDiO.png" width="800">
<img src="https://imgur.com/hDReImQ.png" width="800">
<img src="https://imgur.com/29EZt7d.png" width="800">
<img src="https://imgur.com/kXmLg8V.png" width="800">
<img src="https://imgur.com/tqApMu2.png" width="800">
<img src="https://imgur.com/nfMqFcM.png" width="800">
<img src="https://imgur.com/dQepaRN.png" width="800">

<p><strong>Purpose:</strong> Establishes a dedicated compliance baseline for administrative devices, ensuring that privileged accounts operate on systems that meet higher security standards.</p>

<hr>

<h3>Onboarding My Local PC into Intune</h3>

<img src="https://imgur.com/6FMf98Y.png" width="800">

<p>
  I enrolled my local Windows PC into Intune to test the new compliance policy.
  After enrollment, the device appeared in the Intune portal and began evaluating against the assigned compliance settings.
</p>

<img src="https://imgur.com/BWcR08I.png" width="800">
<img src="https://imgur.com/MUE95H9.png" width="800">

<p><strong>Purpose:</strong> Validates the enrollment process and confirms that the compliance policy is being applied to real devices in the tenant.</p>

<hr>

<h3>Resolving Device Non‑Compliance</h3>

<p>
  After enrollment, my device showed as Non‑compliant due to missing hardware‑based security features such as TPM and BitLocker.
  To resolve this, I updated the compliance policy by disabling the requirements for TPM, BitLocker, and the “Require encryption of data storage on this device” setting.
  Once the policy was updated and the device checked in again, it reported as Compliant.
</p>

<img src="https://imgur.com/wQpn1X2.png" width="800">
<img src="https://imgur.com/xyOCeJ6.png" width="800">
<img src="https://imgur.com/vzMLKmq.png" width="800">
<img src="https://imgur.com/IKSindt.png" width="800">
<img src="https://imgur.com/vzMLKmq.png" width="800">
<img src="https://imgur.com/sgLLf9T.png" width="800">
<img src="https://imgur.com/WbqaE2E.png" width="800">

<p><strong>Purpose:</strong> Demonstrates troubleshooting and policy adjustment skills by identifying non‑compliance causes and modifying the compliance baseline to match the capabilities of the test device.</p>

<hr>

<h3>Creating the “Windows Compliance – Standard Devices” Policy</h3>

<img src="https://imgur.com/BB8DWEu.png" width="800">

<p>
  I created a second compliance policy named “Windows Compliance – Standard Devices.”
  This policy was assigned to the Standard Users security group to provide a separate, less restrictive compliance baseline for non‑admin devices.
</p>

<img src="https://imgur.com/OxGIaUP.png" width="800">
<img src="https://imgur.com/W8WXaCo.png" width="800">
<img src="https://imgur.com/JqadEJo.png" width="800">
<img src="https://imgur.com/GhGlAav.png" width="800">
<img src="https://imgur.com/EIgHKCs.png" width="800">
<img src="https://imgur.com/x2tDA4v.png" width="800">

<p><strong>Purpose:</strong> Separates admin and standard device requirements, allowing for different compliance expectations based on user role and ensuring scalable, role‑appropriate device governance.</p>
