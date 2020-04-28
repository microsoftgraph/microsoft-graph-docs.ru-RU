---
title: Тип ресурса Клаудаппсекуритистате
description: Содержит сведения о состоянии облачного приложения (Дестинатионсервиценаме, Дестинатионсервицеип).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d8e2df4dd25f4209996b4e5cf4f2083790385e84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507644"
---
# <a name="cloudappsecuritystate-resource-type"></a>Тип ресурса Клаудаппсекуритистате

Пространство имен: microsoft.graph

Содержит сведения о состоянии облачного приложения (Дестинатионсервиценаме, Дестинатионсервицеип).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|дестинатионсервицеип|String|Конечный IP-адрес подключения к облачному приложению или службе.|
|дестинатионсервиценаме|String|Имя облачного приложения или службы (например, "Salesforce", "DropBox" и т. д.).|
|riskScore|String|Полученный поставщиком и вычисляемый показатель риска облачного приложения или службы. Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.|

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
