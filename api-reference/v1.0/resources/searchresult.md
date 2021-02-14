---
author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
description: Ресурс SearchResult указывает, что элемент представляет собой отклик на поисковый запрос.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aac8ee9c4dea8ba7744e5c86d865b4d2f75a37d8
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240103"
---
# <a name="searchresult-resource-type"></a>Тип ресурса SearchResult

Пространство имен: microsoft.graph

Ресурс **SearchResult** указывает, что элемент представляет собой отклик на поисковый запрос.

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "onClickTelemtryUrl" ],
  "@odata.type": "microsoft.graph.searchResult"
}-->

```json
{
  "onClickTelemetryUrl": "url"
}
```

## <a name="properties"></a>Свойства

| Свойство            | Тип   | Описание
|:--------------------|:-------|:----------------------------------------------
| onClickTelemetryUrl | Строка | URL-адрес обратного вызова, с помощью которого можно записывать данные телеметрии. Когда пользователь использует этот элемент, приложение должно выполнять запрос GET на этот URL-адрес, чтобы повышать качество результатов.

## <a name="remarks"></a>Заметки 

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

