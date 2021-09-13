---
title: тип ресурсов securityResource
description: Представляет ресурсы, связанные с оповещением.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 377b3828e254676912f549c51aa3776a297edd4b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054074"
---
# <a name="securityresource-resource-type"></a>тип ресурсов securityResource

Пространство имен: microsoft.graph

Представляет ресурсы, связанные с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|resource|String|Имя ресурса, связанного с текущим оповещением. **Обязательное поле**.|
|resourceType|[securityResourceType](#securityresourcetype-values)|Представляет тип ресурсов безопасности, связанных с оповещением. Возможные значения: `attacked`, `related`.|

### <a name="securityresourcetype-values"></a>значения securityResourceType

|Элемент|Значение|Описание|
|-|-|-|
|атаковано|1|Ресурс был атаковат в оповещении.|
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


