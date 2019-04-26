---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: calculatedColumn
localization_priority: Normal
ms.openlocfilehash: e09fab8a6bd59b0a878dfe6c70bd040612ce3b8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328302"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="342e5-102">Тип ресурса calculatedColumn</span><span class="sxs-lookup"><span data-stu-id="342e5-102">CalculatedColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="342e5-103">Ресурс **calculatedColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.</span><span class="sxs-lookup"><span data-stu-id="342e5-103">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="342e5-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="342e5-104">JSON representation</span></span>

<span data-ttu-id="342e5-105">Ниже показано представление ресурса **calculatedColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="342e5-105">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="342e5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="342e5-106">Properties</span></span>

| <span data-ttu-id="342e5-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="342e5-107">Property name</span></span>  | <span data-ttu-id="342e5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="342e5-108">Type</span></span>    | <span data-ttu-id="342e5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="342e5-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="342e5-110">**format**</span><span class="sxs-lookup"><span data-stu-id="342e5-110">**format**</span></span>     | <span data-ttu-id="342e5-111">строка</span><span class="sxs-lookup"><span data-stu-id="342e5-111">string</span></span>  | <span data-ttu-id="342e5-112">Для типов выходных данных `dateTime` это свойство указывает формат значения.</span><span class="sxs-lookup"><span data-stu-id="342e5-112">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="342e5-113">Должно иметь тип `dateOnly` или `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="342e5-113">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="342e5-114">**formula**</span><span class="sxs-lookup"><span data-stu-id="342e5-114">**formula**</span></span>    | <span data-ttu-id="342e5-115">string</span><span class="sxs-lookup"><span data-stu-id="342e5-115">string</span></span>  | <span data-ttu-id="342e5-116">Формула, используемая для вычисления значения для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="342e5-116">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="342e5-117">**outputType**</span><span class="sxs-lookup"><span data-stu-id="342e5-117">**outputType**</span></span> | <span data-ttu-id="342e5-118">string</span><span class="sxs-lookup"><span data-stu-id="342e5-118">string</span></span>  | <span data-ttu-id="342e5-119">Тип выходных данных, используемый для форматирования значений в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="342e5-119">The output type used to format values in this column.</span></span> <span data-ttu-id="342e5-120">Должно иметь один из типов `boolean`, `currency`, `dateTime`, `number` или `text`.</span><span class="sxs-lookup"><span data-stu-id="342e5-120">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="342e5-121">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="342e5-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="342e5-122">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="342e5-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

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
