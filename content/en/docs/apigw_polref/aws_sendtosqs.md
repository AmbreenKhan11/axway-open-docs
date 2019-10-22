{
"title": "Send to Amazon SQS",
"linkTitle": "Send to Amazon SQS",
"date": "2019-10-17",
"description": "Amazon Simple Queue Service (SQS) is a hosted message queuing service for distributing messages amongst machines. API Gateway acts as a client to SQS and can send messages to SQS. You can use the **Send to Amazon SQS**\\nfilter to send messages to an SQS queue."
}
﻿
<div id="p_aws_sendtosqs_overview">

Overview
--------

Amazon Simple Queue Service (SQS) is a hosted message queuing service for distributing messages amongst machines. API Gateway acts as a client to SQS and can send messages to SQS. You can use the **Send to Amazon SQS**
filter to send messages to an SQS queue.

For more information on Amazon SQS, go to <http://aws.amazon.com/sqs/>.

</div>

<div id="p_aws_sendtosqs_config">

General settings
----------------

Configure the following settings on the **Send to Amazon SQS**
window:

**Name**:\
Enter a suitable name for the filter to display in a policy.

<div>

### AWS settings

**AWS Credential**:\
Click the browse button to select your AWS security credentials (API key and secret) for Amazon SQS.

**Region**:\
Select the region in which to access the SQS service. You can choose from the following options:

-   US East (Northern Virginia)
-   US West (Oregon)
-   US West (Northern California)
-   EU (Ireland)
-   Asia Pacific (Singapore)
-   Asia Pacific (Tokyo)
-   Asia Pacific (Sydney)
-   South America (Sao Paulo)
-   US GovCloud

**Client settings**:\
Click the browse button to select the AWS client configuration to be used by API Gateway when connecting to Amazon SQS. For more information on configuring client settings, see
[Configure AWS client settings](/csh?context=601&product=prod-api-gateway-77)
in the
[API Gateway Policy Developer Guide](/bundle/APIGateway_77_PolicyDevGuide_allOS_en_HTML5/)
.

</div>

</div>

<div id="p_aws_sendtosqs_sendmsg">

Send message settings
---------------------

Configure the following settings on the **Send Message**
tab:

**Queue name**:\
Enter the name of the queue to send the message to. The default name is `publishQueue`. To create a new queue with the specified name, click the **Create**
option.

**Send the message payload**:\
Select this option to send the message payload to the queue.

**Or send the value of the attribute below to SQS**:\
Select this option to send the value of an attribute to the queue. Complete the following fields:

-   **Attribute Name**:\
    Enter the name of the attribute.
-   **Content Type**:\
    Enter the content type to be used for sending the message to SQS (for example, `text/plain`).
-   **Content Encoding**:\
    Enter the content encoding.

</div>

<div id="p_aws_sendtosqs_adv">

Advanced settings
-----------------

On the **Advanced**
tab you can configure how to handle messages that are larger than 256KB in size. Configure these fields:

**Split message into smaller ones**:\
Select this option to split the message into smaller messages before sending it to the queue.

**Store in S3 and place pointer on SQS queue**:\
Select this option to store the payload in Amazon S3 and place a pointer to S3 in the queue. Configure the S3 settings as described in [*S3 settings* on page 1](aws_uploadtos3.htm#S3).

</div>

<div id="p_aws_sendtosqs_info">

Further information
-------------------

For more detailed information on Amazon Web Services integration, see the *AWS Integration Guide*
available from Axway Support.

</div>
