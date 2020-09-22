---
title: Тип ресурса Секуритивендоринформатион
description: " поддается подпредоставлению = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 536ed37cfe8ba190a22ef86e190af2b171d352ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983986"
---
# <a name="securityvendorinformation-resource-type"></a>Тип ресурса Секуритивендоринформатион

Пространство имен: microsoft.graph

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

