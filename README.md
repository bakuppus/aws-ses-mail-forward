# aws-ses-mail-forward
Follow instructions as described here: https://aws.amazon.com/blogs/messaging-and-targeting/forward-incoming-email-to-an-external-destination/

Runtime settingsInfo
```
Runtime     :   Python 3.7
HandlerInfo :   lambda_function.lambda_handler
```

Environment variables (5)

The environment variables below are encrypted at rest with the default Lambda service key.
```
Key            Value
====          =======
MailRecipient :	 bakuppus@gmail.com
MailS3Bucket	:  mail.kubelancer.com
MailS3Prefix	:  devops
MailSender	  :  terraform@kubelancer.com
Region	      :  us-east-1
```

Route53

```
	kubelancer.com	MX	Simple		20 inbound-smtp.us-east-1.amazonaws.com
 ```
