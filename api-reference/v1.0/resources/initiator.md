---
title: Тип ресурса инициатора
description: Описывает, кто и что инициировал событие подготовка.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b62c087f8a3519c80c5c3cda0103fd56a2e40f6c5abd0cedf4389270cce85300
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54178411"
---
# <a name="initiator-resource-type"></a>Тип ресурса инициатора

Пространство имен: microsoft.graph

Описывает, кто и что инициировал событие подготовка. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String|Имя лица или службы, которая инициировала событие подготовка.|
|id|String|Уникально идентифицирует человека или службу, которая инициировала событие подготовка.|
|initiatorType|initiatorType| Тип инициатора. Возможные значения: `user`, `application`, `system`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON

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


