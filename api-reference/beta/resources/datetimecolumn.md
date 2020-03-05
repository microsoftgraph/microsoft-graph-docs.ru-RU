---
author: JeremyKelley
description: Ресурс dateTimeColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой даты или время.
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 5c2a90a67a8a283dbc1da497c5824e4eb7ecbc85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507305"
---
# <a name="datetimecolumn-resource-type"></a>Тип ресурса dateTimeColumn

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **dateTimeColumn** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a>Свойства

| Имя свойства      | Тип               | Описание
|:-------------------|:-------------------|:----------------------------------------------
| **displayAs**      | string             | Способ отображения значения в пользовательском интерфейсе. Должно иметь один из типов `default`, `friendly` или `standard`. Дополнительные сведения см. ниже. Если тип не указан, считается, что значение имеет тип `default`.
| **format**         | строка             | Указывает способ представления значения: только в виде даты либо в виде даты и времени. Должно иметь тип `dateOnly` или `dateTime`

## <a name="displayas-values"></a>Значения DisplayAs

| Значение        | Описание
|:-------------|:--------------------------------------------------------------
| **default**  | Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.
| **friendly** | Использование понятного относительного представления (например, "сегодня в 15:00")
| **standard** | Использование стандартного абсолютного представления (например, "10.05.2017 15:20")


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn",
  "suppressions": []
}
-->
