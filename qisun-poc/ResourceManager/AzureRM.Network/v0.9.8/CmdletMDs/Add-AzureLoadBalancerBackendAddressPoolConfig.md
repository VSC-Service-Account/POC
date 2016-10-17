---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Get-AzureLoadBalancer.md
schema: 2.0.0
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/projects/azure-docs-powershell-int/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/CmdletMDs/Add-AzureLoadBalancerBackendAddressPoolConfig.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/projects/azure-docs-powershell-int/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/CmdletMDs/Add-AzureLoadBalancerBackendAddressPoolConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, content
manager: visual-studio-china
---

# Add-AzureLoadBalancerBackendAddressPoolConfig

## SYNOPSIS
Adds a backend address pool configuration to a load balancer.

## SYNTAX

```
Add-AzureLoadBalancerBackendAddressPoolConfig -Name <String> -LoadBalancer <PSLoadBalancer>
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureLoadBalancerBackend** cmdlet adds a backend address pool to an Azure load balancer.

## EXAMPLES

### Example 1 Add a backend address pool configuration to a load balancer
```
PS C:\>Get-AzureLoadBalancer -Name "MyLoadBalancer" -ResourceGroupName "myrg" | Add-AzureLoadBalancerBackendAddressPoolConfig -Name "BackendAddressPool02" | Set-AzureLoadBalancer
```

This command gets the load balancer named MyLoadBalancer, adds the backend address pool named BackendAddressPool02 to MyLoadBalancer, and then uses the **Set-AzureLoadBalancer** cmdlet to update MyLoadBalancer.

## PARAMETERS

### -LoadBalancer
Specifies a **LoadBalancer** object.

```yaml
Type: PSLoadBalancer
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the name of the backend address pool configuration to add.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies an Azure profile.

```yaml
Type: AzureProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureLoadBalancer](.\Get-AzureLoadBalancer.md)

[Get-AzureNetworkInterface](.\Get-AzureNetworkInterface.md)

[Get-AzureLoadBalancerBackendAddressPoolConfig](.\Get-AzureLoadBalancerBackendAddressPoolConfig.md)

[New-AzureLoadBalancerBackendAddressPoolConfig](.\New-AzureLoadBalancerBackendAddressPoolConfig.md)

[Remove-AzureLoadBalancerBackendAddressPoolConfig](.\Remove-AzureLoadBalancerBackendAddressPoolConfig.md)
