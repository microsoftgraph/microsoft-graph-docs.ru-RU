---
title: Тип ресурса Review
description: Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 411de013df02bcd71e851a694664ae010edaf4ab
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597272"
---
# <a name="reviewset-resource-type"></a>Тип ресурса Review

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список рецензентов](../api/reviewset-list.md) | Коллекция [reviewing](reviewset.md) | Получение коллекции наборов проверки. |
| [Получение представления](../api/reviewset-get.md) | [reviewSet](reviewset.md) | Считывание свойств и связей объекта **reviewing** . |
| [Создание представления](../api/reviewset-post.md) | [reviewSet](reviewset.md) | Создайте новый набор рецензирования. |
| [Перечисление запросов](../api/reviewsetquery-list.md)|Коллекция [ревиевсеткуери](../resources/reviewsetquery.md)|Получение ресурсов Ревиевсеткуери из свойства навигации Queries.|
| [Создание запросов](../api/reviewsetquery-post.md)|[reviewSetQuery](../resources/reviewsetquery.md)|Создание нового объекта Ревиевсеткуери.|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy        | [identitySet](/graph/api/resources/identityset) | Пользователь, создавший набор проверки. Только для чтения. |
|createdDateTime  |DateTimeOffset| Дата и время создания набора проверки. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|displayName      |String| Имя набора проверки. Имя уникально с максимальным ограничением в 64 символов. |
|id               |String| Уникальный идентификатор набора проверки. Только для чтения. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
| Просмотр запроса Set |Коллекция [ревиевсеткуери](reviewsetquery.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSet",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
