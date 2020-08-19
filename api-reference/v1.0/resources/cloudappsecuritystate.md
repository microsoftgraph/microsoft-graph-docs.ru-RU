---
title: Тип ресурса Клаудаппсекуритистате
description: Содержит сведения о состоянии облачного приложения (Дестинатионсервиценаме, Дестинатионсервицеип).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ce08f432b980b110defdfa5a9a7816a71f3f7840
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808265"
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

## <a name="json-representation"></a>Представление в формате JSON

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
