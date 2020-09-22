---
author: JeremyKelley
description: Ресурс dateTimeColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой даты или время.
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7de33a9c1f4d6aa3d47495afdbfdb201e74bf11e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050000"
---
# <a name="datetimecolumn-resource-type"></a>Тип ресурса dateTimeColumn

Пространство имен: microsoft.graph

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


