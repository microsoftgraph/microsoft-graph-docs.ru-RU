---
title: Тип ресурса alertTrigger
description: Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991260"
---
# <a name="alerttrigger-resource-type"></a>Тип ресурса alertTrigger

Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|name|String|Имя свойства, используемого в качестве триггера обнаружения.|
|type|String|Тип свойства в пары "ключ: значение" для интерпретации. Например String, Boolean, и т.д.|
|value|String|Значение свойства, используемого в качестве триггера обнаружения.|

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
