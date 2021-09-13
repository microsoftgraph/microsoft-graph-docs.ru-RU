---
author: JeremyKelley
ms.date: 09/11/2017
title: calculatedColumn
ms.localizationpriority: medium
description: Ресурс calculatedColumn в ресурсе columnDefinition указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cfeda60829a12b95bf23ab7ae3c9734baac5a5c4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109516"
---
# <a name="calculatedcolumn-resource-type"></a>Тип ресурса calculatedColumn

Пространство имен: microsoft.graph

Ресурс **calculatedColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление ресурса **calculatedColumn** в формате JSON.
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a>Свойства

| Имя свойства  | Тип    | Описание
|:---------------|:--------|:--------------------------------------------------
| **format**     | строка  | Для типов выходных данных `dateTime` это свойство указывает формат значения. Должно иметь тип `dateOnly` или `dateTime`.
| **formula**    | string  | Формула, используемая для вычисления значения для данного столбца.
| **outputType** | string  | Тип выходных данных, используемый для форматирования значений в этом столбце. Должно иметь один из типов `boolean`, `currency`, `dateTime`, `number` или `text`.

В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.
Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/calculatedcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(boolean,currency,dateTime,number,text) are in resource, but () are in table"
  ],
  "tocPath": "Resources/CalculatedColumn"
} -->

