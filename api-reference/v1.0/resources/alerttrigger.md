---
title: Тип ресурса alertTrigger
description: Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).
author: Preetikr
localization_priority: Normal
ms.openlocfilehash: 1dc8bb2b18380da50134aa67e742da89dea3c057
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894343"
---
# <a name="alerttrigger-resource-type"></a>Тип ресурса alertTrigger

Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|name|Строка|Имя свойства, используемого в качестве триггера обнаружения.|
|type|Строка|Тип свойства в пары "ключ: значение" для интерпретации. Например String, Boolean, и т.д.|
|value|Строка|Значение свойства, используемого в качестве триггера обнаружения.|

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
