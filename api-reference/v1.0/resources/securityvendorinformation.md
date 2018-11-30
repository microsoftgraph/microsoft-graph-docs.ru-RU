---
title: Тип ресурса securityVendorInformation
description: " subProvider = AppLocker)."
ms.openlocfilehash: 0eef5b1d53f4b7b61af0ccede6e02ffc7bdf76ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027329"
---
# <a name="securityvendorinformation-resource-type"></a>Тип ресурса securityVendorInformation

Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|Поставщик |String|Определенного поставщика (продуктов и услуг - не поставщика организации); Например WindowsDefenderATP.|
|providerVersion|String|Версия поставщика или subprovider, если он существует, создавшее оповещение. *Required*|
|subProvider|String|Определенные subprovider (в разделе статистической обработки поставщика); Например WindowsDefenderATP.SmartScreen.|
|поставщика |String|Имя оповещения поставщика (например, Microsoft, Dell, FireEye). *Required*|


## <a name="json-representation"></a>Представление JSON

Соответствовать является представлением JSON ресурса.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
