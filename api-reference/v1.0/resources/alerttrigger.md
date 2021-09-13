---
title: тип ресурса alertTrigger
description: Содержит сведения о свойствах, которые вызвали обнаружение (свойства существуют в объекте оповещений).
author: preetikr
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 78cfe6afd2495291dd3d4b358ab500b41dab25d0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089881"
---
# <a name="alerttrigger-resource-type"></a>тип ресурса alertTrigger

Пространство имен: microsoft.graph

Содержит сведения о свойствах, которые вызвали обнаружение (свойства существуют в объекте оповещений).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|name|String|Имя свойства, которое служит спусковым крючком обнаружения.|
|type|Строка|Тип свойства в паре key:value для интерпретации. Например, String, Boolean и т.д.|
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

