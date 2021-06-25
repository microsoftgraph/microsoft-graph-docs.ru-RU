---
title: тип ресурса alertTrigger
description: Содержит сведения о свойствах, которые вызвали обнаружение (свойства существуют в объекте оповещений).
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6bdee4ee550b44694a572e3611652b19c7ff574c
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129441"
---
# <a name="alerttrigger-resource-type"></a>тип ресурса alertTrigger

Пространство имен: microsoft.graph

Содержит сведения о свойствах, которые вызвали обнаружение (свойства существуют в объекте оповещений).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|name|String|Имя свойства, которое служит спусковым крючком обнаружения.|
|type|String|Тип свойства в паре key:value для интерпретации. Например, String, Boolean и т.д.|
|value|String|Значение свойства, служащая в качестве триггера обнаружения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}
```

## <a name="example"></a>Пример

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

