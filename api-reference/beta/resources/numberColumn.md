---
author: JeremyKelley
description: Ресурс numberColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой числа.
ms.date: 09/11/2017
title: NumberColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
ms.openlocfilehash: 8970c7a2526a4a29a3efe8e27759e81338013ed8
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176925"
---
# <a name="numbercolumn-resource-type"></a>Тип ресурса numberColumn

Пространство имен: microsoft.graph

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

| Свойство          | Тип   | Описание                                                                                                                |
| :---------------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| **decimalPlaces** | string | Количество десятичных разрядов, которые необходимо отображать. Ниже перечислены возможные значения.                                   |
| **displayAs**     | string | Способ отображения значения в пользовательском интерфейсе. Должно иметь тип `number` или `percentage`. Если тип не указан, считается, что значение имеет тип `number`. |
| **maximum**       | double | Максимальное разрешенное значение.                                                                                               |
| **minimum**       | double | Минимальное разрешенное значение.                                                                                               |

## <a name="decimalplaces-values"></a>Значения decimalPlaces

| Значение         | Описание                                              |
| :------------ | :------------------------------------------------------- |
| **automatic** | Значение, используемое по умолчанию. Автоматическое отображение необходимого количества десятичных разрядов. |
| **none**      | Не отображать десятичные разряды.                       |
| **one**       | Всегда отображать один десятичный разряд.                        |
| **two**       | Всегда отображать два десятичных разряда.                       |
| **three**     | Всегда отображать три десятичных разряда.                     |
| **four**      | Всегда отображать четыре десятичных разряда.                      |
| **five**      | Всегда отображать пять десятичных разрядов.                      |

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
