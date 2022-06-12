---
author: JeremyKelley
title: Тип ресурса searchResult
ms.localizationpriority: medium
description: Ресурс searchResult указывает, что элемент является ответом на поисковый запрос.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 376e0a709f7607215aac1b1509434549bd437db3
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034798"
---
# <a name="searchresult-resource-type"></a>Тип ресурса searchResult

Пространство имен: microsoft.graph

Ресурс **searchResult** указывает, что элемент является ответом на поисковый запрос.

## <a name="json-representation"></a>Представление JSON

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

Дополнительные сведения о аспектах в DriveItem см. [в разделе driveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

