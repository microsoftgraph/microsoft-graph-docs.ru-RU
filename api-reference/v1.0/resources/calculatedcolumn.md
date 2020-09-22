---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: calculatedColumn
localization_priority: Normal
description: Ресурс calculatedColumn в ресурсе columnDefinition указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 29699b5f220f4b9e46258a42c3b353cc9712ac6d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066537"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="b3207-103">Тип ресурса calculatedColumn</span><span class="sxs-lookup"><span data-stu-id="b3207-103">CalculatedColumn resource type</span></span>

<span data-ttu-id="b3207-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3207-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b3207-105">Ресурс **calculatedColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.</span><span class="sxs-lookup"><span data-stu-id="b3207-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3207-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b3207-106">JSON representation</span></span>

<span data-ttu-id="b3207-107">Ниже показано представление ресурса **calculatedColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3207-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="b3207-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3207-108">Properties</span></span>

| <span data-ttu-id="b3207-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="b3207-109">Property name</span></span>  | <span data-ttu-id="b3207-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b3207-110">Type</span></span>    | <span data-ttu-id="b3207-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b3207-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="b3207-112">**format**</span><span class="sxs-lookup"><span data-stu-id="b3207-112">**format**</span></span>     | <span data-ttu-id="b3207-113">строка</span><span class="sxs-lookup"><span data-stu-id="b3207-113">string</span></span>  | <span data-ttu-id="b3207-114">Для типов выходных данных `dateTime` это свойство указывает формат значения.</span><span class="sxs-lookup"><span data-stu-id="b3207-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="b3207-115">Должно иметь тип `dateOnly` или `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="b3207-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="b3207-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="b3207-116">**formula**</span></span>    | <span data-ttu-id="b3207-117">string</span><span class="sxs-lookup"><span data-stu-id="b3207-117">string</span></span>  | <span data-ttu-id="b3207-118">Формула, используемая для вычисления значения для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="b3207-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="b3207-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="b3207-119">**outputType**</span></span> | <span data-ttu-id="b3207-120">string</span><span class="sxs-lookup"><span data-stu-id="b3207-120">string</span></span>  | <span data-ttu-id="b3207-121">Тип выходных данных, используемый для форматирования значений в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="b3207-121">The output type used to format values in this column.</span></span> <span data-ttu-id="b3207-122">Должно иметь один из типов `boolean`, `currency`, `dateTime`, `number` или `text`.</span><span class="sxs-lookup"><span data-stu-id="b3207-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="b3207-123">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="b3207-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="b3207-124">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="b3207-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

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

