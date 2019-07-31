---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 06a8d99ba01a8a3fd3d171b800345f81b0819de0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005725"
---
# <a name="resourcereference-resource-type"></a>Тип ресурса Ресаурцереференце

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства [аналитики](officegraphinsights.md).

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
