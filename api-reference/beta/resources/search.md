---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bb38d281895ac11d97a026a4352f68b93e8ba801
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704064"
---
# <a name="search-resource-type"></a>Тип ресурса поиска

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска. Он выступает в качестве привязки к действию [запроса](../api/search-query.md) .

Этот ресурс не должен вызываться таким образом. Любой запрос к ресурсу повлечет некорректный запрос.

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
| [query](../api/search-query.md) | [сеарчреспонсе](searchresponse.md) Семейства| Выполняет запрос, указанный в элементе [сеарчрекуест](../resources/searchrequest.md) |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
