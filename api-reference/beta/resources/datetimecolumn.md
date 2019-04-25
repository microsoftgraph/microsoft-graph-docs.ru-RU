---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
ms.openlocfilehash: da8fe44e377a071ee3f20b82f7190b690dcfd6b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535293"
---
# <a name="datetimecolumn-resource-type"></a>Тип ресурса dateTimeColumn

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
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
