---
title: Тип ресурса securityVendorInformation
description: " subProvider = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fb5dee36da08332fd5c36f7ee4e578cc9fb7deaa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945939"
---
# <a name="securityvendorinformation-resource-type"></a>Тип ресурса securityVendorInformation

Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|Поставщик |Строка|Определенного поставщика (продуктов и услуг - не поставщика организации); Например WindowsDefenderATP.|
|providerVersion|Строка|Версия поставщика или subprovider, если он существует, создавшее оповещение. *Required*|
|subProvider|Строка|Определенные subprovider (в разделе статистической обработки поставщика); Например WindowsDefenderATP.SmartScreen.|
|поставщика |Строка|Имя оповещения поставщика (например, Microsoft, Dell, FireEye). *Required*|


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
