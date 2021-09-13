---
title: тип ресурса resourceReference
description: Сложный тип, содержащий свойства Аналитика.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c7694aa2c9a487a3e07ce99d9850445de26c3acb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123365"
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
| type          | Строка    | Значение строки, которое можно использовать для классификации элемента, например "microsoft.graph.driveItem". |

