---
title: Тип ресурса FilterDatetime
description: Представляет способ фильтрации даты при фильтрации по значениям.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 616f6a67bf761d0346c6d232eb6392ee2dc5fd96
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807761"
---
# <a name="filterdatetime-resource-type"></a>Тип ресурса FilterDatetime

Пространство имен: microsoft.graph

Представляет способ фильтрации даты при фильтрации по значениям.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|дата|string|Дата в формате ISO8601, используемая для фильтрации данных.|
|specificity|string|Точность, с которой производится фильтрация данных на основе даты. Например, если указана дата 2005-04-02, а для свойства specificity задано значение month, после фильтрации останутся все строки, датированные апрелем 2009 г. Допустимые значения: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
