---
external help file: RMAzure_Apimanagement.xml
online version: e067ded3-a2e3-4d53-8628-0ebbafa62721
schema: 2.0.0
updated_at: 10/8/2016 8:32 AM
ms.date: 10/8/2016
ms.topic: reference
source_repo: https://github.com/SummerSun/azure-docs-powershell-int
source_branch: master
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/3c5913303624ba7a7970d6758aac68ea04359cee/azureps-cmdlets-docs/Resource%20Manager/v1.0/AzureRM.APIManagement/Get-AzureRmApiManagementSsoToken.md
---

# Get-AzureRmApiManagementSsoToken
## SYNOPSIS
Gets a link with an SSO token to a deployed management portal of an API Management service.

## SYNTAX

```
Get-AzureRmApiManagementSsoToken -Name <String> -ResourceGroupName <String>
```

## DESCRIPTION
The **Get-AzureRmApiManagementSsoToken** cmdlet returns a link (URL) containing a single sign-on (SSO) token to a deployed management portal of an API Management service.

## EXAMPLES

### Example 1: Get the SSO token of an API Management service
```
PS C:\>Get-AzureRmApiManagementSsoToken -ResourceGroupName "Contoso" -Name "ContosoApi"
```

This command gets the SSO token of an API Management service.

## PARAMETERS

### -Name
Specifies the name of the API Management instance.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of resource group under which API Management exists.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmApiManagement](e067ded3-a2e3-4d53-8628-0ebbafa62721)
