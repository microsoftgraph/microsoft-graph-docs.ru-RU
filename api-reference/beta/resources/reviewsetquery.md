---
title: Тип ресурса Ревиевсеткуери
description: Просмотр запросов Set используется для запроса и отбора данных, хранящихся в представлении "обнаружение электронных данных"
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 7ffea670daffb6c8ce53925096dbd4f2d4986477
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597263"
---
# <a name="reviewsetquery-resource-type"></a>Тип ресурса Ревиевсеткуери

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Просмотр запросов Set используется для запроса и отбора данных, хранящихся в [представлении](reviewset.md)обнаружения электронных данных.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Перечисление запросов](../api/reviewsetquery-list.md) | Коллекция [ревиевсеткуери](reviewsetquery.md) | Перечисление запросов на набор проверок в наборе рецензирования. |
| [Создание запросов](../api/reviewsetquery-post.md) | [reviewSetQuery](reviewsetquery.md) | Создание запроса на проверку набора. |
| [Получение запросов](../api/reviewsetquery-get.md) | [reviewSetQuery](reviewsetquery.md) | Чтение свойств и связей объекта **ревиевсеткуери** . |
| [Запросы на обновление](../api/reviewsetquery-update.md) | Нет | Обновление запроса на проверку набора. |
| [Удаление запросов](../api/reviewsetquery-delete.md) | Нет | Удаление запроса на проверку набора. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| createdBy | [identitySet](/graph/api/resources/identityset) | Пользователь, создавший запрос. |
| createdDateTime |DateTimeOffset| Время и Дата создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
| displayName | String | Имя запроса|
| id |String| Уникальный идентификатор запроса. Только для чтения.|
| lastModifiedBy | [identitySet](/graph/api/resources/identityset) | Пользователь, который последним изменил запрос. |
| lastModifiedDateTime |DateTimeOffset | Дата и время последнего изменения запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
| Запрос | String | Строка запроса в запросе KQL (ключевое слово языка запросов). Дополнительные сведения см. [в статье Field Metadata Fields in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).  Это поле напрямую сопоставляется с условием ключевых слов.  Вы можете уточнить поиск с помощью полей, перечисленных в *имени поля с возможностью поиска* , с указанием значений; Например, *Subject: "квартальное финансовое планирование" и дата>= 06/01/2016 и дата<= 07/01/2016* |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "baseType": "",
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
