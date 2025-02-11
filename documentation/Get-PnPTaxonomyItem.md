---
Module Name: PnP.PowerShell
title: Get-PnPTaxonomyItem
schema: 2.0.0
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
online version: https://pnp.github.io/powershell/cmdlets/Get-PnPTaxonomyItem.html
---
 
# Get-PnPTaxonomyItem

## SYNOPSIS
Returns a taxonomy item

## SYNTAX

```powershell
Get-PnPTaxonomyItem [-TermPath] <String> [-Connection <PnPConnection>]  
 [<CommonParameters>]
```

## DESCRIPTION
Provide the term path only and then the term item if found will be returned.


## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPTaxonomyItem -TermPath "My Term Group|My Term Set|Contoso"
```

Will return the taxonomy item for the term path specified.

## PARAMETERS

### -TermPath
The path, delimited by | of the taxonomy item to retrieve, alike GROUPLABEL|TERMSETLABEL|TERMLABEL

```yaml
Type: String
Parameter Sets: (All)
Aliases: Term

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```
### -Connection
Optional connection to be used by the cmdlet. Retrieve the value for this parameter by either specifying -ReturnConnection on Connect-PnPOnline or by executing Get-PnPConnection.

```yaml
Type: PnPConnection
Parameter Sets: (All)

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## RELATED LINKS

[Microsoft 365 Patterns and Practices](https://aka.ms/m365pnp)

