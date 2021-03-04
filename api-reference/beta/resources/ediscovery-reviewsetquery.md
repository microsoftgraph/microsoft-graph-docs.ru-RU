---
title: reviewSetQuery resource type
description: Представляет запрос набора обзоров, который используется для запроса и отсеить данные, хранимые в обзоре eDiscoverySet.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f9c535cb1adbb62f33aee1324b6dc06a910f4b46
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447362"
---
# <a name="reviewsetquery-resource-type"></a>reviewSetQuery resource type

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запрос набора обзоров, который используется для запроса и отсеить данные, хранимые в обзоре [eDiscoverySet.](ediscovery-reviewset.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Запросы списка](../api/ediscovery-reviewsetquery-list.md) | [коллекция microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | Список запросов набора отзывов в наборе обзоров. |
| [Создание запросов](../api/ediscovery-reviewsetquery-post.md) | [microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | Создайте новый запрос набора обзоров. |
| [Получить запросы](../api/ediscovery-reviewsetquery-get.md) | [microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) | Ознакомьтесь с свойствами и отношениями объекта **reviewSetQuery.** |
| [Обновление обзораSetQuery](../api/ediscovery-reviewsetquery-update.md) | Нет | Обновление запроса набора отзывов. |
| [Удаление просмотретьSetQuery](../api/ediscovery-reviewsetquery-delete.md) | Нет | Удаление запроса набора обзоров. |
| [applyTags](../api/ediscovery-reviewsetquery-applytags.md)|Нет|Применяйте теги к документам, которые соответствуют указанному запросу.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| createdBy | [identitySet](/graph/api/resources/identityset) | Пользователь, создавший запрос. |
| createdDateTime |DateTimeOffset| Время и дата создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
| displayName | String | Имя запроса.|
| id |String| Уникальный идентификатор запроса. Только для чтения.|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | Пользователь, который в последний раз изменил запрос. |
| lastModifiedDateTime |DateTimeOffset | Дата и время последнего изменения запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
| Запрос | String | Строка запроса в запросе KQL (Язык запросов ключевых слов). Дополнительные сведения см. [в материале Поля метаданных документа в advanced eDiscovery.](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)  Это поле совмещеется непосредственно с условием ключевых слов.  Поиск можно уточнить с помощью  полей, перечисленных в имени поля поиска в паре со значениями; например, *subject:"Quarterly Financials" And Date>=06/01/2016 and Date<=07/01/2016*. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSetQuery",
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
