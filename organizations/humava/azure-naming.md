# Azure Naming Convention

## General

| Variable             | Formula                                         |
| -------------------- | ----------------------------------------------- |
| Public Resource Name | ${resourceName}${resourceNumber}${randomSuffix} |
| Environment Name     | prd, tst, dev                                   |
| Region Name          | frcntrl, nrtheu                                 |

## Azure AD

| Variable        | Formula                                                | Example                         |
| --------------- | ------------------------------------------------------ | ------------------------------- |
| Azure AD Tenant | humava${resourceNumber}${randomSuffix}.onmicrosoft.com | humava001gwp665.onmicrosoft.com |

## Azure Resource Manager (ARM)

| Variable                   | Formula                                                                                             | Example               |
| -------------------------- | --------------------------------------------------------------------------------------------------- | --------------------- |
| Resource Group             | rg-${shortApplicationName}-${environmentName}-${regionName}-${resourceNumber}                       | rg-app-dev-nrtheu-001 |
| Log Analytics              | la-${shortApplicationName}-${environmentName}-${regionName}-${resourceNumber}                       | la-app-dev-nrtheu-001 |
| Storage Account            | sa${shortApplicationName}${environmentName}${shortOrganizationName}${resourceNumber}${randomSuffix} | saappdevhva001gwp382  |
| Storage Account File Share |                                                                                                     |                       |