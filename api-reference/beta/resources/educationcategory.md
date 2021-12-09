---
title: тип ресурса educationCategory
description: Категория, которую можно применить к назначениям.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 15c6427062f09493168f0f94cca3060bc3f631de
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390887"
---
# <a name="educationcategory-resource-type"></a>тип ресурса educationCategory

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Категория, которую можно применить к назначениям.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание категории](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | Создание нового **образованияCategory**.|
|[Get educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | Получите существующее **educationCategory**.|
|[Удаление категории](../api/educationcategory-delete.md) | Нет | Удалить **educationCategory**.|
|[Получение дельты](../api/educationcategory-delta.md)|[коллекция educationCategory](../resources/educationcategory.md)|Получите список объектов **educationCategory,** принадлежащих этому классу, с поддержкой запросов delta.|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка|Уникальный идентификатор для категории.|
|displayName|Строка|Уникальный идентификатор для категории.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


