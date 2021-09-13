---
author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
ms.localizationpriority: medium
description: Ресурс SearchResult указывает, что элемент представляет собой отклик на поисковый запрос.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ad26c1df29e78d6c04c4332d5a1c1e9f88c12513
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59126690"
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

