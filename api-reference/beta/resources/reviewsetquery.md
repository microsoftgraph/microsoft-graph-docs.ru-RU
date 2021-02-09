---
title: Тип ресурса reviewSetQuery
description: Запросы набора для проверки используются для запроса и кэша данных, хранимые в наборе отзывов eDiscovery
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f622f79c9103e704be93ffd97af37c1d188736f6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153489"
---
# <a name="reviewsetquery-resource-type"></a>Тип ресурса reviewSetQuery

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запросы набора для проверки используются для запроса и кэш сбор данных, хранимые в наборе отзывов eDiscovery. [](reviewset.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список запросов](../api/reviewsetquery-list.md) | [Коллекция reviewSetQuery](reviewsetquery.md) | Список запросов набора для проверки в наборе для проверки. |
| [Создание запросов](../api/reviewsetquery-post.md) | [reviewSetQuery](reviewsetquery.md) | Создайте запрос набора для проверки. |
| [Получить запросы](../api/reviewsetquery-get.md) | [reviewSetQuery](reviewsetquery.md) | Чтение свойств и связей объекта **reviewSetQuery.** |
| [Обновление запросов](../api/reviewsetquery-update.md) | Нет | Обновление запроса набора для проверки. |
| [Удаление запросов](../api/reviewsetquery-delete.md) | Нет | Удаление запроса набора для проверки. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| createdBy | [identitySet](/graph/api/resources/identityset) | Пользователь, создавший запрос. |
| createdDateTime |DateTimeOffset| Время и дата создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
| displayName | String | Имя запроса|
| id |String| Уникальный идентификатор запроса. Только для чтения.|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | Пользователь, который последним изменил запрос. |
| lastModifiedDateTime |DateTimeOffset | Дата и время последнего изменения запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
| Запрос | String | Строка запроса в KQL (язык запросов по ключевым словам). Дополнительные сведения см. в [полях метаданных документа в Advanced eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)  Это поле сопо карте непосредственно с условием ключевых слов.  Поиск можно уточнить с помощью полей, перечисленных в имени поля для поиска, в *паре* со значениями; например, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016* |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSetQuery",
  "query": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSetQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
