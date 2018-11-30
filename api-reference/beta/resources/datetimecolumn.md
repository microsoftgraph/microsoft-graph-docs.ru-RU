---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: dateTimeColumn
ms.openlocfilehash: 9854ad35c602ff474604f2ca88e7182c325e797d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075531"
---
# <a name="datetimecolumn-resource-type"></a>Тип ресурса dateTimeColumn

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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
| **displayAs**      | строка             | Способ отображения значения в пользовательском интерфейсе. Должно иметь один из типов `default`, `friendly` или `standard`. Дополнительные сведения см. ниже. Если тип не указан, считается, что значение имеет тип `default`.
| **format**         | строка             | Указывает способ представления значения: только в виде даты либо в виде даты и времени. Должно иметь тип `dateOnly` или `dateTime`

## <a name="displayas-values"></a>Значения DisplayAs

| Значение        | Описание
|:-------------|:--------------------------------------------------------------
| **default**  | Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.
| **friendly** | Использование понятного относительного представления (например, "сегодня в 15:00")
| **standard** | Использование стандартного абсолютного представления (например, "10.05.2017 15:20")


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
