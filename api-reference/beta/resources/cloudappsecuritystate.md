---
title: тип ресурсов cloudAppSecurityState
description: Содержит сведения о облачном приложении (destinationServiceName, destinationServiceIp).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 80011803b1e73a4b0377d739c6f0d0b21e38eeb7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126074"
---
# <a name="cloudappsecuritystate-resource-type"></a>тип ресурсов cloudAppSecurityState

Пространство имен: microsoft.graph

Содержит сведения о облачном приложении (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|destinationServiceIp|String|IP-адрес адреса подключения к облачному приложению/службе.|
|destinationServiceName|String|Имя облачного приложения/службы (например, "Salesforce", "DropBox" и т.д.).|
|riskScore|String|Оценка риска, генерируемая поставщиком и рассчитанная для облачного приложения/службы. Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.|

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


