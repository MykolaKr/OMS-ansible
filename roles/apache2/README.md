# Install Apache2 (HTTPD)

Install Apache2 (httpd)  on CentOS

# Variables

Role variable You can change in vars folder.


# Use in playbook

```yaml
  roles:
    - { role: apache2, action: 'install' }
    - { role: apache2, action: 'virtualhost', vhost_name: 'brun', vhost_dir: '/var/www/html/brun' }
    - { role: apache2, action: 'htaccess', username: 'admin', password: 'admin' }
```
                                                                                
Avaible actions:

*install* - Install Apache on Your host(s)
*virtualhost* (params: *vhost_name*, *vhost_dir*) - Create virtual host and folder if not avaible
*htaccess* (params: *username*, *password*) - Create htaccess protection to folder (in progress)
*help* - Show help

# Dependencies

None

# License 

BSD

# Athor

Igor Bronovskyi - @[BrunIF](https://github.com/BrunIF)

Twitter: @[BrunIF](https://twitter.com/BrunIF)

FB: [BrunIF](https://fb.com/BrunIF)

VK: [BrunIF](https://vk.com/BrunIF)
