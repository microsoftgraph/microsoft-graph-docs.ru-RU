---
author: JeremyKelley
ms.date: 09/11/2017
title: calculatedColumn
ms.localizationpriority: medium
description: Ресурс calculatedColumn в ресурсе columnDefinition указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 54c5c37a91cbc8a3d597c33bc4f30f4ead6c4660
ms.sourcegitcommit: 4b852b92535fba8af9b2bbd6f55dc16aced9ef7e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2022
ms.locfileid: "65971604"
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

