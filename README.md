# Ansible Role: Java

Installs Java for RedHat.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values:

    # The defaults provided by this role are specific to each distribution.
    java_packages:
      - java-1.8.0-openjdk

Set the version/development kit of Java to install, along with any other necessary Java packages. Some other options include are included in the distribution-specific files in this role's 'defaults' folder.

    java_home: ""

If set, the role will set the global environment variable `JAVA_HOME` to this value.

## Dependencies

None.

## Example Playbook (install OpenJDK 8)

    - hosts: server
      roles:
        - role: 
           - java
          java_packages:
            - java-1.8.0-openjdk


## License

VWGoA.

## Author Information

Automation and Innovation Team.
