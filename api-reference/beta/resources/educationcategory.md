---
title: Тип ресурса Едукатионкатегори
description: Категория, которая может быть применена к назначениям.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: dd9eccac3a1b6b1bdc3b0eca4c87b5e29e2135a9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536178"
---
# <a name="educationcategory-resource-type"></a>Тип ресурса Едукатионкатегори

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Категория, которая может быть применена к назначениям.


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Едукатионкатегори](../api/educationcategory-get.md) | [Едукатионкатегори](educationcategory.md) | Получение существующего **едукатионкатегори**.|
|[Удаление категории](../api/educationcategory-delete.md) | Нет | Удаление **едукатионкатегори**.|


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
