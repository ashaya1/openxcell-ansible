## ReactJs+Nginx Deployment

- Requires Ansible 1.2 or newer
- Expects CentOS/RHEL 6.x hosts

These playbooks deploy a simple all-in-one configuration of the popular
Simple React App, frontend by the Nginx web server. To use, copy the `hosts.example` file to `hosts` and 
edit the `hosts` inventory file to include the names or URLs of the servers
you want to deploy.

Then run the playbook, like this:

	ansible-playbook -i hosts site.yml

The playbooks will configure ReactJs, and Nginx. When the run
is complete, you can hit access server url dashboard to check the application hosted.

Dashboard URL: http://app.192.168.0.10.nip.io/

### Ideas for Improvement

Here are some ideas for ways that these playbooks could be extended:

- Parameterize the ReactJs Nginx server url in configuration deployment to handle configurations.

We would love to see contributions and improvements, so please fork this
repository on GitHub and send us your changes via pull requests.