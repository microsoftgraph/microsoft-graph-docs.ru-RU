---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: 5e8bcbc18975758586b012ee32fb32ce15313517
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876603"
---
# <a name="searchresult-resource-type"></a>Тип ресурса SearchResult

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
