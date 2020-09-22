---
title: Тип ресурса Алерттригжер
description: Содержит сведения о свойствах, которые активируют обнаружение (свойства, существующие в объекте Alert).
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e99bb19af970eea2b062748ed41a0d62cb3a02b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041703"
---
# <a name="alerttrigger-resource-type"></a>Тип ресурса Алерттригжер

Пространство имен: microsoft.graph

Содержит сведения о свойствах, которые активируют обнаружение (свойства, существующие в объекте Alert).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|name|String|Имя свойства, служащего триггером обнаружения.|
|type|String|Тип свойства в соотношении "ключ: значение" для интерпретации. Например, String, Boolean и т. д.|
|value|String|Значение свойства, служащего триггером обнаружения.|

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

