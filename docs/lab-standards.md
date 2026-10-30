# Lab Standards

These rules apply to every project in this portfolio. They follow Microsoft's Cloud Adoption Framework guidance.

## Region
- Primary: **East US**
- Secondary (for replication and disaster recovery demos): **East US 2**

## Naming convention
Format: `<resource type>-<workload>-<environment>-<region>-<instance>`

| Resource | Prefix | Example |
| --- | --- | --- |
| Resource group | `rg` | `rg-az104-p12-dev` |
| Virtual network | `vnet` | `vnet-hub-eus` |
| Subnet | `snet` | `snet-web` |
| Network security group | `nsg` | `nsg-web` |
| Virtual machine | `vm` | `vm-web-dev-eus-01` |
| Public IP | `pip` | `pip-vm-web` |
| Load balancer | `lbe` / `lbi` | `lbe-web-dev` |
| Storage account | `st` (no dashes, lowercase) | `stresumejf` |
| Log Analytics workspace | `law` | `law-lab-eus` |
| Recovery Services vault | `rsv` | `rsv-lab-eus` |

## Required tags
| Tag | Example | Why |
| --- | --- | --- |
| `project` | `p12` | Track cost per project |
| `env` | `lab` | Separate lab from anything else |
| `owner` | `jfreeman` | Know who to ask |

## Cost rules
1. Monthly budget with alerts at 50%, 80% and 100%.
2. One resource group per project, deleted when the project is finished.
3. Auto-shutdown on every VM.
4. Use the cheapest SKU that demonstrates the skill.
