---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version:
schema: 2.0.0
content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Get-AzureRmApplicationGatewayRedirectConfiguration.md
original_content_git_url: https://github.com/Azure/azure-powershell/blob/preview/src/ResourceManager/Network/Commands.Network/help/Get-AzureRmApplicationGatewayRedirectConfiguration.md
gitcommit: https://github.com/Azure/azure-powershell/blob/ae060e9ea34c37f2cde2b7c1e2aacff632b227c2
---

# Get-AzureRmApplicationGatewayRedirectConfiguration

## SYNOPSIS
Gets an existing redirect configuration from an Application Gateway.

## SYNTAX

```
Get-AzureRmApplicationGatewayRedirectConfiguration [-Name <String>] -ApplicationGateway <PSApplicationGateway>
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmApplicationGatewayRedirectConfiguration** cmdlet gets an existing redirect configuration from an Application Gateway.

## EXAMPLES

### Example 1
```
PS C:\>$AppGW = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $RedirectConfig = Get-AzureRmApplicationGatewayRedirectConfiguration -Name "Redirect01" -ApplicationGateway $AppGW
```

The first command gets the Application Gateway named ApplicationGateway01 and stores the result in the variable named $AppGW.
The second command gets the redirect configuration named Redirect01 from the Application Gateway stored in the variable named $AppGW.

## PARAMETERS

### -ApplicationGateway
The applicationGateway

```yaml
Type: PSApplicationGateway
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
The name of the request routing rule

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGateway

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayRedirectConfiguration
System.Collections.Generic.IEnumerable`1[[Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayRedirectConfiguration, Microsoft.Azure.Commands.Network, Version=4.1.0.0, Culture=neutral, PublicKeyToken=null]]

## NOTES

## RELATED LINKS

