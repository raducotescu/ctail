# rsyslog example

The rsyslog config file [add-priority-text.conf](add-priority-text.conf) has the necessary config to add 
syslog-priority-text to the logline produced by rsyslog. The important part of the config is
`[%syslogpriority-text%]`.

You can copy the config file to /etc/rsyslog.d/03-add-priority-text.conf and restart `rsyslog` service.

Now you need to copy the [ctail config](ctail.config) to your home directory.

That's it! Now you should be able to colourise logs using the command

    ctail -f /var/log/messages
