---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: a30a1fe5891a0f8a58f08d742ef2aac645006156
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985797"
---
# <a name="search-resource-type"></a>Тип ресурса поиска

Пространство имен: microsoft.graph

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


