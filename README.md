# Ansible Collection - community.memsource

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

This collection aims to offer an Ansible native experience in order to interact and automate workflows with [Memsouce](https://www.memsource.com/). - "Helping global companies translate efficiently"

## Included content

### Modules

Name | Description
--- | ---
[memsource_import_settings](./plugins/memsource_import_settings.py) | Manage a Memsource import settings configuration
[memsource_import_settings_info](./plugins/memsource_import_settings_info.py) | List all available Memsource import settings configurations
[memsource_job](./plugins/memsource_job.py) | Manage a Memsource job
[memsource_job_info](./plugins/memsource_job_info.py) | List all Memsource job
[memsource_job_targetfile](./plugins/memsource_job_targetfile.py) | Download a Memsource job target file
[memsource_project](./plugins/memsource_project.py) | Manage a Memsource project
[memsource_project_info](./plugins/memsource_project_info.py) | List all Memsource projects available
[memsource_project_template_info](./plugins/memsource/project_template_info.py) | List all Memsource project templates available

## Installing this collection

You can install the AWS collection with the Ansible Galaxy CLI:

```sh
#> ansible-galaxy collection install community.memsource
```

You can also include it in a `requirements.yml` file and install it with `ansible-galaxy collection install -r requirements.yml`, using the format:

```yaml
---
collections:
  - name: community.memsource
```

The python module dependencies are not installed by `ansible-galaxy`.  They can
be manually installed using pip:

```sh
#> pip install requirements.txt
```

or:

```sh
pip install python-memsource
```

## Using this collection


You can either call modules by their Fully Qualified Collection Namespace (FQCN), such as `community.memsource.memsource_project`, or you can call modules by their short name if you list the `community.memsource` collection in the playbook's `collections` keyword:

```yaml
---
  - name: Gather all projects
    community.memsource.memsource_project_info:
      filters:
        name: Foo
    register: projects
```

### Authentication

There are two supported ways for a user to authenticate with the Memsource API:

* Using the environment variables `$MEMSOURCE_USERNAME` and `$MEMSOURCE_PASSWORD`
* Using the per task level configuration modules `memsource_username` and `memsource_password`

## Contributing to this collection

We welcome community contributions to this collection. If you find problems, please open an issue or create a PR against the [Memsource collection repository](https://github.com/ansible/ansible-collection-memsource).

See [Contributing to Ansible-maintained collections](https://docs.ansible.com/ansible/devel/community/contributing_maintained_collections.html#contributing-maintained-collections) for more details.


# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License
* Nho Luong (c). All Rights Reserved.🌟