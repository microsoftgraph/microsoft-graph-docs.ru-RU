---
title: Тип ресурса cloudAppSecurityState
description: Содержит сведения об облачном приложении с отслеживанием состояния (destinationServiceName, destinationServiceIp).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: d509aa92fafb3848a5bb77c5f4fb1b0674d66f31
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420756"
---
# <a name="cloudappsecuritystate-resource-type"></a>Тип ресурса cloudAppSecurityState

Пространство имен: microsoft.graph

Содержит сведения об облачном приложении с отслеживанием состояния (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|destinationServiceIp|String|IP-адрес назначения подключения к облачному приложению или службе.|
|destinationServiceName|String|Имя облачного приложения или службы (например, Salesforce, DropBox и т. д.).|
|riskScore|String|Созданная поставщиком или вычисляемая оценка риска для облачного приложения или службы. Рекомендуемый диапазон значений — 0–1, что соответствует проценту.|

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


