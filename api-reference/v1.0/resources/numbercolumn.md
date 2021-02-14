---
author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
description: Ресурс numberColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой числа.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 89b5c81f94895e248dfd4c5f75983bacf352f9e8
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238633"
---
# <a name="numbercolumn-resource-type"></a>Тип ресурса numberColumn

Пространство имен: microsoft.graph

Ресурс **numberColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой числа.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **numberColumn** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.numberColumn" } -->

```json
{
  "decimalPlaces": "automatic | none | one | two | three | four | five",
  "displayAs": "number | percentage",
  "maximum": 10.551,
  "minimum": 99.993
}
```

## <a name="properties"></a>Свойства

| Имя свойства      | Тип   | Описание
|:-------------------|:-------|:-----------------------------------------------
| **decimalPlaces**  | string | Количество десятичных разрядов, которые необходимо отображать. Ниже перечислены возможные значения.
| **displayAs**      | string | Способ отображения значения в пользовательском интерфейсе. Должно иметь тип `number` или `percentage`. Если тип не указан, считается, что значение имеет тип `number`.
| **maximum**        | double | Максимальное разрешенное значение.
| **minimum**        | double | Минимальное разрешенное значение.

## <a name="decimalplaces"></a>DecimalPlaces

| Значение          | Описание
|:---------------|:--------------------------------------------------------------
| **automatic**  | Значение, используемое по умолчанию. Автоматическое отображение необходимого количества десятичных разрядов.
| **none**       | Не отображать десятичные разряды.
| **one**        | Всегда отображать один десятичный разряд.
| **two**        | Всегда отображать два десятичных разряда.
| **three**      | Всегда отображать три десятичных разряда.
| **four**       | Всегда отображать четыре десятичных разряда.
| **five**       | Всегда отображать пять десятичных разрядов.

Примечание. Свойства **decimalPlaces** и **displayAs** указывают способ отображения значений, а не то, в каком виде они хранятся.
Эти свойства можно обновлять.

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(automatic,none,one,two,three,four,five) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/numbercolumn.md:
      Found potential enums in resource example that weren't defined in a table:(number,percentage) are in resource, but () are in table"
  ],
  "tocPath": "Resources/NumberColumn"
} -->

