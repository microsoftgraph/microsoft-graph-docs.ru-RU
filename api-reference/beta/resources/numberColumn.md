---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: NumberColumn
ms.openlocfilehash: 27d17d3e9b9d3d1debcd20f2beb916222801ebe9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082433"
---
# <a name="numbercolumn-resource-type"></a>Тип ресурса numberColumn

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
| **decimalPlaces**  | строка | Количество десятичных разрядов, которые необходимо отображать. Ниже перечислены возможные значения.
| **displayAs**      | строка | Способ отображения значения в пользовательском интерфейсе. Должно иметь тип `number` или `percentage`. Если тип не указан, считается, что значение имеет тип `number`.
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/NumberColumn"
} -->
