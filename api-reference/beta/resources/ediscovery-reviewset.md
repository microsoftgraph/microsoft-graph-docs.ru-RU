---
title: тип ресурса reviewSet
description: Представляет статический набор сведений, хранимых в электронной форме, собранных для использования в судебном, следственном или нормативном запросе.
ms.localizationpriority: medium
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c8e7f51e32a48556ece3d5bfd34b3224b50b8b70
ms.sourcegitcommit: e75969aa44a1aab722ac44d09c37508ffbad8738
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2021
ms.locfileid: "61307624"
---
# <a name="reviewset-resource-type"></a>тип ресурса reviewSet

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет статический набор сведений, хранимых в электронной форме, собранных для использования в судебном, следственном или нормативном запросе.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List reviewSets](../api/ediscovery-case-list-reviewsets.md) | [коллекция microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Получите коллекцию **объектов reviewSet.** |
| [Создание reviewSet](../api/ediscovery-case-post-reviewsets.md) | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Создание нового **reviewSet**. |
| [Get reviewSet](../api/ediscovery-reviewset-get.md) | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Ознакомьтесь с свойствами и отношениями объекта **reviewSet.** |
| [Запросы списка](../api/ediscovery-reviewsetquery-list.md)|[коллекция microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md)|Получите список ресурсов **reviewSetQuery.**|
| [экспорт](../api/ediscovery-reviewset-export.md) | Нет | Инициировать экспорт данных из **наборов отзывов.** |
| [addToReviewSet](../api/ediscovery-reviewset-addtoreviewset.md)|Нет|Добавление данных из **sourceCollection в** **набор отзывов.**|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy        | [identitySet](/graph/api/resources/identityset) | Пользователь, создавший набор отзывов. Только для чтения. |
|createdDateTime  |DateTimeOffset| Дата создания набора отзывов. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
|displayName      |Строка| Имя набора обзоров. Имя уникально с максимальным ограничением в 64 символа. |
|id               |Строка| В обзоре установлен уникальный идентификатор. Только для чтения. |

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
| запросы |[коллекция microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSet",
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
