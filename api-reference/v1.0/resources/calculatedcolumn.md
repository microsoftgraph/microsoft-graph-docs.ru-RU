---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: calculatedColumn
localization_priority: Normal
description: Ресурс calculatedColumn в ресурсе columnDefinition указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 19f11c7033f03dbf4a190acbd6df54bbdfe1fa24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029976"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="98af2-103">Тип ресурса calculatedColumn</span><span class="sxs-lookup"><span data-stu-id="98af2-103">CalculatedColumn resource type</span></span>

<span data-ttu-id="98af2-104">Ресурс **calculatedColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.</span><span class="sxs-lookup"><span data-stu-id="98af2-104">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98af2-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="98af2-105">JSON representation</span></span>

<span data-ttu-id="98af2-106">Ниже показано представление ресурса **calculatedColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98af2-106">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="98af2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="98af2-107">Properties</span></span>

| <span data-ttu-id="98af2-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="98af2-108">Property name</span></span>  | <span data-ttu-id="98af2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="98af2-109">Type</span></span>    | <span data-ttu-id="98af2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="98af2-110">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="98af2-111">**format**</span><span class="sxs-lookup"><span data-stu-id="98af2-111">**format**</span></span>     | <span data-ttu-id="98af2-112">строка</span><span class="sxs-lookup"><span data-stu-id="98af2-112">string</span></span>  | <span data-ttu-id="98af2-113">Для типов выходных данных `dateTime` это свойство указывает формат значения.</span><span class="sxs-lookup"><span data-stu-id="98af2-113">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="98af2-114">Должно иметь тип `dateOnly` или `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="98af2-114">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="98af2-115">**formula**</span><span class="sxs-lookup"><span data-stu-id="98af2-115">**formula**</span></span>    | <span data-ttu-id="98af2-116">string</span><span class="sxs-lookup"><span data-stu-id="98af2-116">string</span></span>  | <span data-ttu-id="98af2-117">Формула, используемая для вычисления значения для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="98af2-117">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="98af2-118">**outputType**</span><span class="sxs-lookup"><span data-stu-id="98af2-118">**outputType**</span></span> | <span data-ttu-id="98af2-119">string</span><span class="sxs-lookup"><span data-stu-id="98af2-119">string</span></span>  | <span data-ttu-id="98af2-120">Тип выходных данных, используемый для форматирования значений в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="98af2-120">The output type used to format values in this column.</span></span> <span data-ttu-id="98af2-121">Должно иметь один из типов `boolean`, `currency`, `dateTime`, `number` или `text`.</span><span class="sxs-lookup"><span data-stu-id="98af2-121">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="98af2-122">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="98af2-122">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="98af2-123">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="98af2-123">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

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
