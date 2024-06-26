<!-- BEGIN_ANSIBLE_DOCS -->

# Ansible Role: ansible-role-create_testing_ad_domain
DEPRECATED: Use trippsc2.ad.testing_domain_controller instead.

## Requirements

| Platform | Versions |
| -------- | -------- |
| Windows | <ul><li>2019</li><li>2022</li></ul> |

## Dependencies

| Collection |
| ---------- |
| microsoft.ad |

## Role Arguments
|Option|Description|Type|Required|Choices|Default|
|---|---|---|---|---|---|
| dc_initial_dns_servers | List of initial DNS servers to use when creating the domain. | list of 'str' | no |  | ["8.8.8.8", "1.1.1.1"] |
| domain_name | The name of the domain to create. | str | no |  | test.loc |
| dc_safe_mode_password | The password to use for the domain in safe mode. | str | no |  | SecurePassword123! |
| dc_domain_admin_username | The username to which to give all administrative rights for the domain. | str | no |  | vagrant |
| dc_domain_admin_password | The password for the domain admin user. If not provided, the domain admin user must already exist. | str | no |  |  |
| domain_base_dn | The base DN for the domain. | str | no |  | DC=test,DC=loc |


## License
MIT

## Author and Project Information
Jim Tarpley
<!-- END_ANSIBLE_DOCS -->
