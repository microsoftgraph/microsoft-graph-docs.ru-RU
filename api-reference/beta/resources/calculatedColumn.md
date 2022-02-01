---
author: JeremyKelley
description: Ресурс calculatedColumn в ресурсе columnDefinition указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.
ms.date: 09/11/2017
title: calculatedColumn
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 232afda8b37ddd5307a32a8e9636f184cf7e6613
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62290604"
---
# <a name="calculatedcolumn-resource-type"></a>Тип ресурса calculatedColumn

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": []
}
-->


