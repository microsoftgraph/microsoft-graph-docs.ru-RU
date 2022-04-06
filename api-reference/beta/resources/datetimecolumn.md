---
author: JeremyKelley
description: Ресурс dateTimeColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой даты или время.
ms.date: 09/11/2017
title: dateTimeColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: adca775df47110f5d79cf9b85c8877f05d22a361
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/22/2022
ms.locfileid: "63724107"
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

| Свойство      | Тип   | Описание                                                                                                                                                         |
| :------------ | :----- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **displayAs** | string | Способ отображения значения в пользовательском интерфейсе. Должно иметь один из типов `default`, `friendly` или `standard`. Дополнительные сведения см. ниже. Если тип не указан, считается, что значение имеет тип `default`. |
| **format**    | строка | Указывает способ представления значения: только в виде даты либо в виде даты и времени. Должно иметь тип `dateOnly` или `dateTime`                                          |

## <a name="displayas-values"></a>Значения DisplayAs

| Значение        | Описание                                                         |
| :----------- | :------------------------------------------------------------------ |
| **default**  | Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.                               |
| **friendly** | Использование понятного относительного представления (например, "сегодня в 15:00")    |
| **standard** | Использование стандартного абсолютного представления (например, "10.05.2017 15:20") |

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
