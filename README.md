ansible-awstats
=========
Install and configure awstats as a log parser, similar to [Logstash](https://www.elastic.co/products/logstash).


Requirements
------------
Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.


Role Variables
--------------

**awstats_analyzed:** Array of log files to analyze with awstats. Default: `[]`

```yaml
awstats_analyzed:
	- log: /var/log/squid/combined.log
	- log: /var/log/apache/foo_site/access.log
```


Dependencies
------------
A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.


Example Playbook
----------------
Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }


License
-------
MIT


Author Information
------------------
Feel free to contact me on [twitter](https://twitter.com/devynspencer) with questions, suggestions, or criticisms. Alternatively, [open a ticket](https://github.com/devynspencer/ansible-awstats/issues/new) and I'll do my best to integrate your feedback!
