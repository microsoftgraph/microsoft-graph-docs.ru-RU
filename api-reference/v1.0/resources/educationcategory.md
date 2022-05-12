---
title: Тип ресурса educationCategory
description: Категория, которую можно применить к назначениям.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2a265a8733b72dc26967b390503abdbf201d9a1e
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65365913"
---
# <a name="educationcategory-resource-type"></a>Тип ресурса educationCategory

Пространство имен: microsoft.graph

Категория, которую можно применить к назначениям.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание категории](../api/educationclass-post-category.md) | [educationCategory](educationcategory.md) | Создайте **новую educationCategory**.|
|[Получение educationCategory](../api/educationcategory-get.md) | [educationCategory](educationcategory.md) | Получите существующую **educationCategory**.|
|[Удаление категории](../api/educationcategory-delete.md) | Нет | Удалите **educationCategory**.|
|[Получение дельты](../api/educationcategory-delta.md)|[Коллекция educationCategory](../resources/educationcategory.md)|Получение списка вновь созданных или обновленных объектов **educationCategory** без необходимости выполнять полное чтение коллекции.|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|Уникальный идентификатор категории.|
|displayName|String|Уникальный идентификатор категории.|

## <a name="json-representation"></a>Представление в формате JSON

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


