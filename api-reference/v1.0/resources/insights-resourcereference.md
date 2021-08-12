---
title: тип ресурса resourceReference
description: Сложный тип, содержащий свойства Аналитика.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7ade1e86fc601d1f00a16136a8610634934d0b4faf7b377a85ff55cf65fab671
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152623"
---
# <a name="resourcereference-resource-type"></a>тип ресурса resourceReference

Пространство имен: microsoft.graph

Сложный тип, содержащий свойства [officeGraphInsights.](officegraphinsights.md)

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
| webUrl        | String    | URL-адрес, ведущий к ссылке элемента. |
| id            | String    | Уникальный идентификатор элемента.           |
| type          | String    | Значение строки, которое можно использовать для классификации элемента, например "microsoft.graph.driveItem". |

