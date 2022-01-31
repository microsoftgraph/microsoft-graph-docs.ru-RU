---
title: Тип ресурса поиска
description: Объект верхнего уровня, представляющем конечную точку поиска в Microsoft Graph.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 034e1adec8d1bcee0336abdbeed2d980ee559964
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282050"
---
# <a name="search-resource-type"></a>Тип ресурса поиска

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объект верхнего уровня, представляющем конечную точку поиска. Он служит якорем для [действия запроса](../api/search-query.md) .

Этот ресурс не называется. Любой запрос, который вызывает этот ресурс, приведет к http-ответу `400 Bad Request` .

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [query](../api/search-query.md) | [коллекция searchResponse](searchresponse.md)| Запустите указанный поисковый запрос. |

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Нет.

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


