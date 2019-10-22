{
"title": "Configure XKMS connections",
"linkTitle": "Configure XKMS connections",
"date": "2019-10-17",
"description": "XML Key Management Specification (XKMS) is an XML-based protocol that enables you to establish the trustworthiness of a certificate over the Internet. The API Gateway can query an XKMS responder to determine whether a given certificate can be trusted."
}
﻿
<div id="p_certificate_xkms_connection_overview">

Overview
--------

XML Key Management Specification (XKMS) is an XML-based protocol that enables you to establish the trustworthiness of a certificate over the Internet. The API Gateway can query an XKMS responder to determine whether a given certificate can be trusted.

You can add XKMS Connections under the **Environment Configuration** > **External Connections**
tree node in Policy Studio. To add a global XKMS Connection, right-click the **XKMS Connections**
node, and select **Add an XKMS Connection**.

</div>

<div id="p_certificate_xkms_connection_conf">

Configuration
-------------

Configure the following fields on the **Certificate Validation - XKMS**
window.

**Name**:\
Enter an appropriate name for this XKMS connection.

**URL Group**:\
Select a group of XKMS responders from the URL Group list. The API Gateway attempts to connect to the XKMS responders in the selected group in a round-robin fashion. It attempts to connect to the responders with the highest priority first, before connecting to responders with a lower priority.

You can add, edit, or remove URL Groups by selecting the appropriate button. For more information on adding and editing URL groups, see [*Configure URL groups* on page 1](common_url_groups.htm).

**User Name**:\
Requests to XKMS responders can be signed by a user to whom the **Sign OCSP or XKMS Requests**
privilege has been assigned. Only those users who have been assigned this privilege are displayed in the drop-down list. For more information on assigning privileges to users, see [*Manage users* on page 1](../CommonTopics/general_users.htm).

**Signing Key**:\
Click the **Signing Key**
button to open the list of certificates in the Certificate Store. You can then select the key to use to sign requests to XKMS responders. This user must have been granted the Sign OCSP or XKMS Requests privilege.

</div>
