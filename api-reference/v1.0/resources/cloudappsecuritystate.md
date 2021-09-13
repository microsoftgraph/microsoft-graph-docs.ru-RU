---
title: тип ресурсов cloudAppSecurityState
description: Содержит сведения о облачном приложении (destinationServiceName, destinationServiceIp).
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d04a23bb38c9f5264057d56d43de0f053dd58b9c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118759"
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

