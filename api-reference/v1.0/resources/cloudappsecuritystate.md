---
title: Тип ресурса cloudAppSecurityState
description: Содержит сведения об облачном приложении с отслеживанием состояния (destinationServiceName, destinationServiceIp).
ms.localizationpriority: medium
author: preetikr
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: b367766b7605a0c0444c17d962e9e034269683f2
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65970939"
---
# <a name="cloudappsecuritystate-resource-type"></a>Тип ресурса cloudAppSecurityState

Пространство имен: microsoft.graph

Содержит сведения об облачном приложении с отслеживанием состояния (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|destinationServiceIp|Строка|IP-адрес назначения подключения к облачному приложению или службе.|
|destinationServiceName|Строка|Имя облачного приложения или службы (например, Salesforce, DropBox и т. д.).|
|riskScore|Строка|Созданная поставщиком или вычисляемая оценка риска для облачного приложения или службы. Рекомендуемый диапазон значений — 0–1, что соответствует проценту.|

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

