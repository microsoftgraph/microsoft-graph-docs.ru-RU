---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: calculatedColumn
ms.openlocfilehash: a5850961e680459af27f3e76965f0d3e1c97e923
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081252"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="3e38f-102">Тип ресурса calculatedColumn</span><span class="sxs-lookup"><span data-stu-id="3e38f-102">CalculatedColumn resource type</span></span>

> <span data-ttu-id="3e38f-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e38f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e38f-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e38f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e38f-105">Ресурс **calculatedColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.</span><span class="sxs-lookup"><span data-stu-id="3e38f-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e38f-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3e38f-106">JSON representation</span></span>

<span data-ttu-id="3e38f-107">Ниже показано представление ресурса **calculatedColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e38f-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="3e38f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e38f-108">Properties</span></span>

| <span data-ttu-id="3e38f-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="3e38f-109">Property name</span></span>  | <span data-ttu-id="3e38f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3e38f-110">Type</span></span>    | <span data-ttu-id="3e38f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3e38f-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="3e38f-112">**format**</span><span class="sxs-lookup"><span data-stu-id="3e38f-112">**format**</span></span>     | <span data-ttu-id="3e38f-113">строка</span><span class="sxs-lookup"><span data-stu-id="3e38f-113">string</span></span>  | <span data-ttu-id="3e38f-114">Для типов выходных данных `dateTime` это свойство указывает формат значения.</span><span class="sxs-lookup"><span data-stu-id="3e38f-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="3e38f-115">Должно иметь тип `dateOnly` или `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="3e38f-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="3e38f-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="3e38f-116">**formula**</span></span>    | <span data-ttu-id="3e38f-117">строка</span><span class="sxs-lookup"><span data-stu-id="3e38f-117">string</span></span>  | <span data-ttu-id="3e38f-118">Формула, используемая для вычисления значения для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="3e38f-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="3e38f-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="3e38f-119">**outputType**</span></span> | <span data-ttu-id="3e38f-120">строка</span><span class="sxs-lookup"><span data-stu-id="3e38f-120">string</span></span>  | <span data-ttu-id="3e38f-121">Тип выходных данных, используемый для форматирования значений в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="3e38f-121">The output type used to format values in this column.</span></span> <span data-ttu-id="3e38f-122">Должно иметь один из типов `boolean`, `currency`, `dateTime`, `number` или `text`.</span><span class="sxs-lookup"><span data-stu-id="3e38f-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="3e38f-123">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="3e38f-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="3e38f-124">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="3e38f-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn"
} -->
