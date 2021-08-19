---
title: тип ресурсов securityResource
description: Представляет ресурсы, связанные с оповещением.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: f8beb524375db5fc4187f210b8602e534835a53f3dc9c52b60ee57085f904ce2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212936"
---
# <a name="securityresource-resource-type"></a>тип ресурсов securityResource

Пространство имен: microsoft.graph

Представляет ресурсы, связанные с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|resource|Строка|Имя ресурса, связанного с текущим оповещением. **Обязательное поле**.|
|resourceType|[securityResourceType](#securityresourcetype-values)|Представляет тип ресурсов безопасности, связанных с оповещением. Возможные значения: `attacked`, `related`.|

### <a name="securityresourcetype-values"></a>значения securityResourceType

|Элемент|Значение|Описание|
|-|-|-|
|атаковано|1 |Ресурс был атаковат в оповещении.|
|связанные|2|Ресурс связан с оповещением, но не напрямую атаковал.|

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


