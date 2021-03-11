---
title: тип ресурса reviewSet
description: Представляет статический набор сведений, хранимых в электронной форме, собранных для использования в судебном, следственном или нормативном запросе.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: bcb21fece207e9e4d98fa7a0fc612f886e5ab0e6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720338"
---
# <a name="reviewset-resource-type"></a>тип ресурса reviewSet

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет статический набор сведений, хранимых в электронной форме, собранных для использования в судебном, следственном или нормативном запросе.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [List reviewSets](../api/ediscovery-case-list-reviewsets.md) | [коллекция microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Получите коллекцию объектов **reviewset.** |
| [Создание reviewSet](../api/ediscovery-case-post-reviewsets.md) | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Создайте новый **обзор.** |
| [Get reviewSet](../api/ediscovery-reviewset-get.md) | [microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) | Ознакомьтесь с свойствами и отношениями объекта **reviewSet.** |
| [Запросы списка](../api/ediscovery-reviewsetquery-list.md)|[коллекция microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md)|Получите список ресурсов **reviewSetQuery.**|
| [экспорт](../api/ediscovery-reviewset-export.md) | Нет | Инициировать экспорт данных из **наборов отзывов.** |
| [addToReviewSet](../api/ediscovery-reviewset-addtoreviewset.md)|Нет|Добавление данных из **sourceCollection в** **набор отзывов.**|

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdBy        | [identitySet](/graph/api/resources/identityset) | Пользователь, создавший набор отзывов. Только для чтения. |
|createdDateTime  |DateTimeOffset| Дата создания набора отзывов. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Только для чтения. |
|displayName      |String| Имя набора обзоров. Имя уникально с максимальным ограничением в 64 символа. |
|id               |String| В обзоре установлен уникальный идентификатор. Только для чтения. |

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
