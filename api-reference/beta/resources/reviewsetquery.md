---
title: Тип ресурса Ревиевсеткуери
description: Просмотр запросов Set используется для запроса и отбора данных, хранящихся в представлении "обнаружение электронных данных"
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 2030d2f3403af2967100cbbc7de2571b8493895d
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510385"
---
# <a name="reviewsetquery-resource-type"></a>Тип ресурса Ревиевсеткуери

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Просмотр запросов Set используется для запроса и отбора данных, хранящихся в [представлении](reviewset.md)обнаружения электронных данных.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/reviewsetquery-list.md) | Коллекция [ревиевсеткуери](reviewsetquery.md) | Перечисление запросов на набор проверок в наборе рецензирования. |
| [создание](../api/reviewsetquery-post.md); | [ревиевсеткуери](reviewsetquery.md) | Создание запроса на проверку набора. |
| [получение](../api/reviewsetquery-get.md); | [ревиевсеткуери](reviewsetquery.md) | Чтение свойств и связей объекта **ревиевсеткуери** . |
| [обновление](../api/reviewsetquery-update.md). | Нет | Обновление запроса на проверку набора. |
| [удаление](../api/reviewsetquery-delete.md); | Нет | Удаление запроса на проверку набора. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| createdBy | [identitySet](https://docs.microsoft.com/graph/api/resources/identityset) | Пользователь, создавший запрос. |
| createdDateTime |DateTimeOffset| Время и Дата создания запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
| displayName | Строка | Имя запроса|
| id |String| Уникальный идентификатор запроса. Только для чтения.|
| lastModifiedBy | [identitySet](https://docs.microsoft.com/graph/api/resources/identityset) | Пользователь, который последним изменил запрос. |
| lastModifiedDateTime |DateTimeOffset | Дата и время последнего изменения запроса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
| Запрос | Строка | Строка запроса в запросе KQL (ключевое слово языка запросов). https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscoveryДополнительные сведения см.  Это поле напрямую сопоставляется с условием ключевых слов.  Вы можете уточнить поиск с помощью полей, перечисленных в *имени поля с возможностью поиска* , с указанием значений, например *Subject: "ежеквартальные финансовые операции" и "дата>= 06/01/2016 и дата<= 07/01/2016* |

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
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "query": "String"
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
