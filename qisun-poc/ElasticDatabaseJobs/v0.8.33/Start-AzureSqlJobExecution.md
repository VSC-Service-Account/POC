---
external help file: Microsoft.Azure.SqlDatabase.Jobs.PowerShell.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 0E2D8FAD-FAB9-46BF-81BB-5631C0EE2006
updated_at: 11/17/2016 5:33 AM
ms.date: 11/17/2016
content_git_url: https://github.com/SummerSun/azure-docs-powershell-int/blob/master/azureps-cmdlets-docs/ElasticDatabaseJobs/v0.8.33/Start-AzureSqlJobExecution.md
gitcommit: https://github.com/SummerSun/azure-docs-powershell-int/blob/2692a7998846b66d06a416c56978167da402f8d5/azureps-cmdlets-docs/ElasticDatabaseJobs/v0.8.33/Start-AzureSqlJobExecution.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ElasticDatabaseJobs_v0_8_33_Start_AzureSqlJobExecution_md
---

# Start-AzureSqlJobExecution

## SYNOPSIS
Starts a job execution.

## SYNTAX

```
Start-AzureSqlJobExecution -JobName <String[]> [[-AzureSqlJobConnection] <AzureSqlJobConnection>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureSqlJobExecution** cmdlet starts a job execution.

## EXAMPLES

### Example 1: Start a job execution using a specified job name
```
PS C:\>Start-AzureSqlJobExecution -JobName "MyJob"
JobExecutionId       : 736de27d-186f-42ae-8a4c-e5a77c683ccd
ParentJobExecutionId :
Lifecycle            : Created
CreatedTime          : 7/10/2015 2:15:32 PM -07:00
StartTime            :
EndTime              :
JobName              : MyJob
ContentName          : MyScript
ContentVersionNumber : 1
TargetDescription    : {"CustomCollectionName":"myCustomCollection"}
TargetId             : b525727e-6ed0-44cc-94da-63c543e383d7
CredentialName       : MyCredential
ExecutionPolicyName  : Default execution policy
ResultSetDestination :
```

This command starts a job execution using the job named MyJob.

## PARAMETERS

### -AzureSqlJobConnection
Specifies the connection state object for the job.
You can get the connection state object through the [New-AzureSqlJobConnection](./New-AzureSqlJobConnection.md) cmdlet.
If you do not specify this parameter, the connection state is used from a prior call to the [Use-AzureSqlJobConnection](./Use-AzureSqlJobConnection.md) cmdlet.

```yaml
Type: AzureSqlJobConnection
Parameter Sets: (All)
Aliases:

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobName
Specifies the name of the job.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureSqlJobExecution](xref:ElasticDatabaseJobs/v0.8.33/Get-AzureSqlJobExecution.md)

[Stop-AzureSqlJobExecution](xref:ElasticDatabaseJobs/v0.8.33/Stop-AzureSqlJobExecution.md)

[Wait-AzureSqlJobExecution](xref:ElasticDatabaseJobs/v0.8.33/Wait-AzureSqlJobExecution.md)

[Azure Elastic Database Jobs Cmdlets](xref:ElasticDatabaseJobs/v0.8.33/ElasticDatabaseJobs.md)