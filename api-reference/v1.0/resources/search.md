---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8e9d8bc133a050701543f2a978e56b662bafcc33
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378041"
---
# <a name="search-resource-type"></a>Тип ресурса поиска

Пространство имен: microsoft.graph

Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска. Он выступает в качестве привязки к действию [запроса](../api/search-query.md) .

Этот ресурс не должен вызываться таким образом. Любой запрос к ресурсу повлечет некорректный запрос.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a>Представление в формате JSON

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


