---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: NumberColumn
localization_priority: Normal
ms.openlocfilehash: f70a1d71729be68fc4d5dcb3de2599ff131bb8a9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342095"
---
# <a name="numbercolumn-resource-type"></a>Тип ресурса numberColumn

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

## <a name="decimalplaces-values"></a>Значения decimalPlaces

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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn",
  "suppressions": []
}
-->
