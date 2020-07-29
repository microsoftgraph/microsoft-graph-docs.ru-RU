---
title: Тип ресурса Review
description: Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 374984f2d44050c1332ec016f83a1ccdea909ba0
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510168"
---
# <a name="reviewset-resource-type"></a>Тип ресурса Review

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список](../api/reviewset-list.md) | Коллекция [reviewing](reviewset.md) | Получение коллекции наборов проверки. |
| [получение](../api/reviewset-get.md); | [проверяющий](reviewset.md) | Считывание свойств и связей объекта **reviewing** . |
| [создание](../api/reviewset-post.md); | [проверяющий](reviewset.md) | Создайте новый набор рецензирования. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy| [identitySet](https://docs.microsoft.com/graph/api/resources/identityset) | Пользователь, создавший набор проверки. Только для чтения. |
|createdDateTime|DateTimeOffset| Дата и время создания набора проверки. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Только для чтения. |
|displayName|Строка| Имя набора проверки. Имя уникально с максимальным ограничением в 64 символов. |
|id|String| Уникальный идентификатор набора проверки. Только для чтения. |

## <a name="relationships"></a>Отношения

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
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)"
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
