---
title: Тип ресурса Секуритивендоринформатион
description: " поддается подпредоставлению = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d7af6e0903e3d178bacdd7c86b4a2cab04285171
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536099"
---
# <a name="securityvendorinformation-resource-type"></a>Тип ресурса Секуритивендоринформатион

Содержит сведения о продуктах, поставщиках и подценнях безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подпредоставление = AppLocker).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|поставщики |String|Конкретный поставщик (продукт или услуга — не компания поставщика); Например, Виндовсдефендератп.|
|провидерверсион|String|Версия поставщика или подсистемы, если она существует, создавшего оповещение. *Required*|
|подпредоставление|String|Конкретный подпредоставленный поставщик (в разделе Поставщик статистической обработки); Например, Виндовсдефендератп. SmartScreen.|
|поставщика |String|Имя поставщика оповещений (например, Microsoft, Dell, Фирие). *Required*|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
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
