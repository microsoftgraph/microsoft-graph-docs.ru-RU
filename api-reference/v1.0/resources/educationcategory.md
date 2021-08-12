---
title: тип ресурса educationCategory
description: Категория, которую можно применить к назначениям.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1b8454265c7c01b7e9a27653e06e0d383d0e7f944f451adc55e5688faecaa79a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130368"
---
# <a name="educationcategory-resource-type"></a>тип ресурса educationCategory

Пространство имен: microsoft.graph

Категория, которую можно применить к назначениям.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание категории](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | Создание нового **образованияCategory**.|
|[Get educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | Получите существующее **educationCategory**.|
|[Удаление категории](../api/educationcategory-delete.md) | Нет | Удалить **educationCategory**.|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|Уникальный идентификатор для категории.|
|displayName|String|Уникальный идентификатор для категории.|

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


