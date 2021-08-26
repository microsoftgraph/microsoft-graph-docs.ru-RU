---
title: Тип ресурса policyBase
description: Представляет абстрактный базовый тип для типов политик, от которые можно наследовать.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2918543536f62627f7c2a742009c3d67012353b4
ms.sourcegitcommit: 998c63e6290cfb5ad4a6bd3eb3e249d282f962a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2021
ms.locfileid: "58531224"
---
# <a name="policybase-resource-type"></a>Тип ресурса policyBase

Пространство имен: microsoft.graph

Представляет абстрактный базовый тип для типов политик, от которые можно наследовать. Наследуется от [directoryObject](directoryobject.md).

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Уникальный идентификатор для этой политики. Только для чтения. Наследуется от [directoryObject](directoryobject.md).|
|description|String| Описание этой политики.|
|displayName|String| Отображение имени для этой политики. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policyBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
