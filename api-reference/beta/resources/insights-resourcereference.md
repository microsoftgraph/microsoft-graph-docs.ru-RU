---
title: Тип ресурса Ресаурцереференце
description: Сложный тип, содержащий свойства аналитики.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2992895b2fbc426d4177dd86074dcf5cb8d784ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495867"
---
# <a name="resourcereference-resource-type"></a>Тип ресурса Ресаурцереференце

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства [оффицеграфинсигхтс](officegraphinsights.md).

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
