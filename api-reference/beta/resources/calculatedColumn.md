---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: calculatedColumn
localization_priority: Normal
ms.openlocfilehash: b3a0d76a236cc4bce53bf476a90e8f37757ae003
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512628"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="aa1e6-102">Тип ресурса calculatedColumn</span><span class="sxs-lookup"><span data-stu-id="aa1e6-102">CalculatedColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa1e6-103">Ресурс **calculatedColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-103">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa1e6-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aa1e6-104">JSON representation</span></span>

<span data-ttu-id="aa1e6-105">Ниже показано представление ресурса **calculatedColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="aa1e6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa1e6-106">Properties</span></span>

| <span data-ttu-id="aa1e6-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="aa1e6-107">Property name</span></span>  | <span data-ttu-id="aa1e6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aa1e6-108">Type</span></span>    | <span data-ttu-id="aa1e6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aa1e6-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="aa1e6-110">**format**</span><span class="sxs-lookup"><span data-stu-id="aa1e6-110">**format**</span></span>     | <span data-ttu-id="aa1e6-111">string</span><span class="sxs-lookup"><span data-stu-id="aa1e6-111">string</span></span>  | <span data-ttu-id="aa1e6-112">Для типов выходных данных `dateTime` это свойство указывает формат значения.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="aa1e6-113">Должно иметь тип `dateOnly` или `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="aa1e6-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="aa1e6-114">**formula**</span></span>    | <span data-ttu-id="aa1e6-115">string</span><span class="sxs-lookup"><span data-stu-id="aa1e6-115">string</span></span>  | <span data-ttu-id="aa1e6-116">Формула, используемая для вычисления значения для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="aa1e6-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="aa1e6-117">**outputType**</span></span> | <span data-ttu-id="aa1e6-118">string</span><span class="sxs-lookup"><span data-stu-id="aa1e6-118">string</span></span>  | <span data-ttu-id="aa1e6-119">Тип выходных данных, используемый для форматирования значений в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-119">The output type used to format values in this column.</span></span> <span data-ttu-id="aa1e6-120">Должно иметь один из типов `boolean`, `currency`, `dateTime`, `number` или `text`.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="aa1e6-121">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="aa1e6-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="aa1e6-122">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="aa1e6-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/calculatedColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
