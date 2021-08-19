---
title: тип ресурсов cloudAppSecurityState
description: Содержит сведения о облачном приложении (destinationServiceName, destinationServiceIp).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f5b82357d91889aada97c835fcab2c327c05fe143988a9ed3bf47ee293687770
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253770"
---
# <a name="cloudappsecuritystate-resource-type"></a>тип ресурсов cloudAppSecurityState

Пространство имен: microsoft.graph

Содержит сведения о облачном приложении (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|destinationServiceIp|Строка|IP-адрес адреса подключения к облачному приложению/службе.|
|destinationServiceName|Строка|Имя облачного приложения/службы (например, "Salesforce", "DropBox" и т.д.).|
|riskScore|Строка|Оценка риска, генерируемая поставщиком и рассчитанная для облачного приложения/службы. Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|

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


