---
external help file: AdminUI.PS.HS.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 70F90D3C-9019-4AE8-9CFC-693D9D3AC351
---

# New-CMFileReplicationRoute

## SYNOPSIS
Creates a file replication route for Configuration Manager.

## SYNTAX

```
New-CMFileReplicationRoute -SourceSiteCode <String> -DestinationSiteCode <String>
 [-DestinationSiteServerName <String>] [-FileReplicationAccountName <String>] [-DisableWildcardHandling]
 [-ForceWildcardHandling] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **New-CMFileReplicationRoute** cmdlet creates a file replication route for Microsoft System Center Configuration Manager.
System Center Configuration Manager uses file replication routes to transfer file-based data between sites in a hierarchy.
Each file replication route identifies a destination site to which file-based data can transfer.

File replication routes were known as addresses in versions of Configuration Manager before System Center Configuration Manager.
The functionality of file replication routes is the same as that of addresses in earlier versions.

## EXAMPLES

### Example 1: Create a file replication route
```
PS C:\>New-CMFileReplicationRoute -DestinationSiteCode "IM5" -SourceSiteCode "IM1" -DestinationSiteServerName "ImgDataServer01" -FileReplicationAccountName "AdminRepl01"
```

This command creates a file replication route from the site that has the site code IM1 to the site that has the site code IM5 on the server named ImgDataServer01.
System Center Configuration Manager uses the account named AdminRepl01 to manage data transfer over this route.

## PARAMETERS

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -DestinationSiteCode


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

### -DestinationSiteServerName


```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DisableWildcardHandling
Indicates that wildcard handling is disabled.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FileReplicationAccountName


```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ForceWildcardHandling
Indicates that wildcard handling is enabled.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourceSiteCode


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

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-CMFileReplicationRoute](./Get-CMFileReplicationRoute.md)

[Remove-CMFileReplicationRoute](./Remove-CMFileReplicationRoute.md)

[Set-CMFileReplicationRoute](./Set-CMFileReplicationRoute.md)

