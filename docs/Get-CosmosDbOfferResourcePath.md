---
external help file: CosmosDB-help.xml
Module Name: CosmosDB
online version:
schema: 2.0.0
---

# Get-CosmosDbOfferResourcePath

## SYNOPSIS

Return the resource path for a offer object.

## SYNTAX

```powershell
Get-CosmosDbOfferResourcePath [-Id] <String> [<CommonParameters>]
```

## DESCRIPTION

This cmdlet returns the resource identifier for a offer
object.

## EXAMPLES

### Example 1

```powershell
PS C:\> Get-CosmosDbOfferResourcePath -Id '6teb'
```

Generate a resource path for offer '6teb'.

## PARAMETERS

### -Id

This is the Id of the offer.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### System.String

## NOTES

## RELATED LINKS
