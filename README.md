---
title: Buildah build
subtitle: Ansible Galaxy 
---

# Role Name


Build container images with Buildah using Ansible.

## Requirements


Buildah installed

## Role Variables


Depending on the task being executed it has different variables.

### commit

| Variable | Meaning |
| --- | --- |
| container_name | Name of the container being commited |
| image_name | Name of the image to create from the container |
| buildah_commit | Result of the commit execution |


## Dependencies

None

## Example Playbook

### Commit

```yaml
  - name: Check if container image exists
    include_role:
      name: "buildah-build"
      tasks_from: "inspect"
    vars:
      image_name: "{{ image-name }}"
```

## License

BSD

## Author Information

Trikora Solutions SL

[url: www.trikorasolutions.com](http://www.trikorasolutions.com/)

[Linkedin - Trikora Solutions](https://www.linkedin.com/company/trikora-solutions-sl/)

[Linkedin - A.C.](linkd.in/ajcin/)

[Twitter - @trikorasolns](https://twitter.com/trikorasolns)

