---
title: Тип ресурса Секуритиресаурце
description: Представляет ресурсы, связанные с оповещением.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ce0398ba134f7537420a99ccaed84f2ff209f883
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682021"
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
|связываем|2|Ресурс связан с оповещением, хотя и не может напрямую атаковаться.|

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
