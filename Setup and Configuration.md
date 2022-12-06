Setup and Configuration

- An Orchestrator Queue in the same folder as the process is required. By default, the automation will look for a queue named "SMA". This queue name can be changed in either the config file or the in argument of the process (will override the config value).
- By default, unread emails will be pulled from the Inbox folder of the local Outlook app and marked as read after being added to the queue. If demoing, it is advisable to create a separate folder to be processed instead to avoid your emails getting marked as read. The folder used by the process can be updated either in the config file or the "in_MailFolder" argument to the process.
- By default, processed emails will not be moved to another folder. To move emails to another folder, specify a "ProcessedEmailsMailFolder" value inside the config or process argument with the same name.
- Only unread emails are pulled by the dispatcher. Ensure the mails you are targeting are unread before running.