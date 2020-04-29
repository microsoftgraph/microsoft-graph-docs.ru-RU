---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
description: Ресурс SearchResult указывает, что элемент представляет собой отклик на поисковый запрос.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f3f3c9edceb864e8e1f895ccdfe4e5a4f8e6046a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446949"
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
