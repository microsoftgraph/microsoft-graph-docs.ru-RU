---
title: тип ресурса educationCategory
description: Категория, которую можно применить к назначениям.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b4bd1220e65b2c855d4698cbe24f1d4d8d9f6ac7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025568"
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


