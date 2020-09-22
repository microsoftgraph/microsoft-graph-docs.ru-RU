---
title: Тип ресурса Клаудаппсекуритистате
description: Содержит сведения о состоянии облачного приложения (Дестинатионсервиценаме, Дестинатионсервицеип).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0f987f64960290c4104ed1c0746ce38591cb3ab6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086797"
---
# <a name="cloudappsecuritystate-resource-type"></a>Тип ресурса Клаудаппсекуритистате

Пространство имен: microsoft.graph

Содержит сведения о состоянии облачного приложения (Дестинатионсервиценаме, Дестинатионсервицеип).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|дестинатионсервицеип|Строка|Конечный IP-адрес подключения к облачному приложению или службе.|
|дестинатионсервиценаме|Строка|Имя облачного приложения или службы (например, "Salesforce", "DropBox" и т. д.).|
|riskScore|Строка|Полученный поставщиком и вычисляемый показатель риска облачного приложения или службы. Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

