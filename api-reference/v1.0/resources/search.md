---
title: Поиск
description: Извлечение ресурса поиска, используемой для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7f20a7d0513f084dadc8dc3f3693a7dd51109fb7e9ccbb163a80a17a29d6978f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251810"
---
# <a name="search-resource-type"></a>Тип ресурса поиска

Пространство имен: microsoft.graph

Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска. Он служит якорем для [действия запроса.](../api/search-query.md)

Этот ресурс не будет называться как таковой. Любой запрос на ресурс будет понести bad request.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a>Представление JSON

Нет

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

Нет

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [query](../api/search-query.md) | [searchResponse](searchresponse.md) Коллекция| Выполняет запрос, указанный в [searchRequest](../resources/searchrequest.md) |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


