---
title: Тип ресурса Секуритиресаурце
description: Представляет ресурсы, связанные с оповещением.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 4d27b5815366bdce76e5f99f0410f67684e608ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988823"
---
# <a name="securityresource-resource-type"></a>Тип ресурса Секуритиресаурце

Пространство имен: microsoft.graph

Представляет ресурсы, связанные с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|resource|String|Имя ресурса, связанного с текущим оповещением. **Обязательное поле**.|
|Ресурса|[секуритиресаурцетипе](#securityresourcetype-values)|Представляет тип ресурсов безопасности, связанных с оповещением. Возможные значения: `attacked`, `related`.|

### <a name="securityresourcetype-values"></a>значения Секуритиресаурцетипе

|Элемент|Значение|Описание|
|-|-|-|
|атаковать|1 |Ресурс был атакован в оповещении.|
|связываем|2 |Ресурс связан с оповещением, хотя и не может напрямую атаковаться.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.securityResource"
}-->

```json
{
  "resource": "String",
  "resourceType": "@odata.type: microsoft.graph.securityResourceType"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


