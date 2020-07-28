---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fac5ec3b40467034a583933a6e09399e91badfe0
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427398"
---
# <a name="resourcereference-resource-type"></a>Тип ресурса Ресаурцереференце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства [итеминсигхтс](iteminsights.md)

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>Свойства

| Свойство      | Тип      | Описание  |
| ------------- |-----------| -------------|
| webUrl        | String    | URL-адрес, ведущая к указанному элементу. |
| id            | Строка    | Уникальный идентификатор элемента.           |
| type          | String    | Строковое значение, которое может использоваться для классификации элемента, например "Microsoft. Graph. driveItem" |
