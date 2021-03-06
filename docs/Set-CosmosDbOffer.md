---
external help file: CosmosDB-help.xml
Module Name: CosmosDB
online version:
schema: 2.0.0
---

# Set-CosmosDbOffer

## SYNOPSIS

Update an existing offer in a Cosmos DB database.

## SYNTAX

### Context (Default)

```powershell
Set-CosmosDbOffer -Context <Context> [-Key <SecureString>] -InputObject <Object[]> [-OfferVersion <String>]
 [-OfferType <String>] [-OfferThroughput <Int32>] [-OfferIsRUPerMinuteThroughputEnabled <Boolean>]
 [<CommonParameters>]
```

### Account

```powershell
Set-CosmosDbOffer -Account <String> [-Key <SecureString>] [-KeyType <String>] -InputObject <Object[]>
 [-OfferVersion <String>] [-OfferType <String>] [-OfferThroughput <Int32>]
 [-OfferIsRUPerMinuteThroughputEnabled <Boolean>] [<CommonParameters>]
```

## DESCRIPTION

This cmdlet will update an offer resource in Cosmos DB.

## EXAMPLES

### Example 1

```powershell
Get-CosmosDbOffer -Context $cosmosDbContext -Id 'lyiu' | Set-CosmosDbOffer -Context $cosmosDbContext -OfferThroughput 1000 -OfferIsRUPerMinuteThroughputEnabled $true
```

Update an existing V2 offer with the Id 'lyiu' to set a different throughput.

## PARAMETERS

### -Account

The account name of the Cosmos DB to access.

```yaml
Type: String
Parameter Sets: Account
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Context

This is an object containing the context information of the Cosmos DB database
that will be deleted. It should be created by \`New-CosmosDbContext\`.

```yaml
Type: Context
Parameter Sets: Context
Aliases: Connection

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InputObject

This must contain one oo more offer records to update.

```yaml
Type: Object[]
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Key

The key to be used to access this Cosmos DB.

```yaml
Type: SecureString
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -KeyType

The type of key that will be used to access ths Cosmos DB.

```yaml
Type: String
Parameter Sets: Account
Aliases:
Accepted values: master, resource

Required: False
Position: Named
Default value: Master
Accept pipeline input: False
Accept wildcard characters: False
```

### -OfferIsRUPerMinuteThroughputEnabled

The offer is RU per minute throughput enabled.
Applicable for V2 offers only.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -OfferThroughput

This contains the throughput of the collection.
Applicable for V2 offers only.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
```

### -OfferType

This is a user settable property, which must be set to S1, S2, or S3 for
pre-defined performance levels, and Invalid for user-defined performance
levels.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Accepted values: S1, S2, S3, Invalid

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OfferVersion

This can be V1 for pre-defined throughput levels and V2 for user-defined
throughput levels.

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Accepted values: V1, V2

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

### System.Object

## NOTES

## RELATED LINKS
