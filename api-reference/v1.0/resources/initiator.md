---
title: Тип ресурса инициатора
description: Описывает, кто и что инициировал событие подготовка.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b1450b8344907f321b4620a909561fb5253b26b0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240775"
---
# <a name="initiator-resource-type"></a>Тип ресурса инициатора

Пространство имен: microsoft.graph

Описывает, кто и что инициировал событие подготовка. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|Строка|Имя лица или службы, которая инициировала событие подготовка.|
|id|Строка|Уникально идентифицирует человека или службу, которая инициировала событие подготовка.|
|initiatorType|initiatorType| Тип инициатора. Возможные значения: `user`, `application`, `system`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.initiator",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "id": "String",
  "initiatorType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "initiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


