---
title: Тип ресурса Секуритивендоринформатион
description: " подДается подПредоставлению = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fb5dee36da08332fd5c36f7ee4e578cc9fb7deaa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549701"
---
# <a name="securityvendorinformation-resource-type"></a>Тип ресурса Секуритивендоринформатион

Содержит сведения о продуктах, поставщиках и подценнях безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подПредоставление = AppLocker).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|поставщики |String|Конкретный поставщик (продукт или услуга — не компания поставщика); Например, Виндовсдефендератп.|
|Провидерверсион|String|Версия поставщика или подСистемы, если она существует, создавшего оповещение. *Required*|
|подПредоставление|String|Конкретный подпредоставленный поставщик (в разделе Поставщик статистической обработки); Например, Виндовсдефендератп. SmartScreen.|
|поставщика |String|Имя поставщика оповещений (например, Microsoft, Dell, Фирие). *Required*|


## <a name="json-representation"></a>Представление в формате JSON

Следующем — это представление ресурса в формате JSON.
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
