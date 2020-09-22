---
title: Тип ресурса Едукатионкатегори
description: Категория, которая может быть применена к назначениям.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82ad4f009ca76625c148e8a42e58385195466fbb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095543"
---
# <a name="educationcategory-resource-type"></a>Тип ресурса Едукатионкатегори

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Категория, которая может быть применена к назначениям.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание категории](../api/educationclass-post-category.md) | [едукатионкатегори](educationcategory.md) | Создание нового **едукатионкатегори**.|
|[Получение Едукатионкатегори](../api/educationcategory-get.md) | [едукатионкатегори](educationcategory.md) | Получение существующего **едукатионкатегори**.|
|[Удаление категории](../api/educationcategory-delete.md) | Нет | Удаление **едукатионкатегори**.|


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка|Уникальный идентификатор для категории.|
|displayName|Строка|Уникальный идентификатор для категории.|

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
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
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


