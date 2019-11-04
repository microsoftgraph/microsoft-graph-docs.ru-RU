---
title: Поиск
description: Получение поискового ресурса, используемого для выполнения запросов
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 65a099ea0ae57b116bcf6a251170e507945226c9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938774"
---
# <a name="search-resource-type"></a>Тип ресурса поиска

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс поиска — это объект верхнего уровня, представляющий конечную точку поиска. Он выступает в качестве привязки к действию [запроса](../api/search-query.md) .

Этот ресурс не должен вызываться таким образом. Любой запрос к ресурсу повлечет некорректный запрос.

## <a name="json-representation"></a>Представление JSON

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

Нет

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [подчинен](../api/search-query.md) | [сеарчреспонсе](searchresponse.md) Семейства| Выполняет запрос, указанный в элементе [сеарчрекуест](../resources/searchrequest.md) |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
