---
external help file: AdminUI.PS.AppMan.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: C77E2084-F298-4B89-AA9B-89A8DB91715D
---

# Get-CMApplicationRevisionHistory

## SYNOPSIS
Gets a Configuration Manager object that represents the revision history for an application.

## SYNTAX

### SearchBySingleNameMandatory (Default)
```
Get-CMApplicationRevisionHistory [-Name] <String> [-Revision <UInt32>] [-DisableWildcardHandling]
 [-ForceWildcardHandling] [<CommonParameters>]
```

### SearchByValueMandatory
```
Get-CMApplicationRevisionHistory -InputObject <IResultObject> [-Revision <UInt32>] [-DisableWildcardHandling]
 [-ForceWildcardHandling] [<CommonParameters>]
```

### SearchBySingleIdMandatory
```
Get-CMApplicationRevisionHistory -Id <Int32> [-Revision <UInt32>] [-DisableWildcardHandling]
 [-ForceWildcardHandling] [<CommonParameters>]
```

## DESCRIPTION
The **Get-CMApplicationRevisionHistory** cmdlet gets a Microsoft System Center Configuration Manager object that represents the revision history for an application.
When you revise an application or a deployment type contained in an application, System Center Configuration Manager creates a new revision of the application.
You can use the revision history to display each revision made to an application, view the properties of a revision, restore a previous revision, or delete an old revision.

## EXAMPLES

### Example 1: Get the revision history for an application
```
PS C:\>Get-CMApplicationRevisionHistory -Name "MSXML 6.0 Parser"
```

This command gets the application revision history named MSXML 6.0 Parser.

## PARAMETERS

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

### -Id


```yaml
Type: Int32
Parameter Sets: SearchBySingleIdMandatory
Aliases: CIId, CI_ID

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject
Specifies an application object.
To obtain an application object, use the Get-CMApplication cmdlet.

```yaml
Type: IResultObject
Parameter Sets: SearchByValueMandatory
Aliases: Application

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name


```yaml
Type: String
Parameter Sets: SearchBySingleNameMandatory
Aliases: LocalizedDisplayName

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Revision


```yaml
Type: UInt32
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

[Remove-CMApplicationRevisionHistory](./Remove-CMApplicationRevisionHistory.md)

[Restore-CMApplicationRevisionHistory](./Restore-CMApplicationRevisionHistory.md)

