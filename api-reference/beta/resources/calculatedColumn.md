---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: calculatedColumn
localization_priority: Normal
ms.openlocfilehash: 5433b5b5a76d313f8f34e460400906479e6d3d7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876057"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="f07c3-102">Тип ресурса calculatedColumn</span><span class="sxs-lookup"><span data-stu-id="f07c3-102">CalculatedColumn resource type</span></span>

> <span data-ttu-id="f07c3-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f07c3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f07c3-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f07c3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f07c3-105">Ресурс **calculatedColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.</span><span class="sxs-lookup"><span data-stu-id="f07c3-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f07c3-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f07c3-106">JSON representation</span></span>

<span data-ttu-id="f07c3-107">Ниже показано представление ресурса **calculatedColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f07c3-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="f07c3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f07c3-108">Properties</span></span>

| <span data-ttu-id="f07c3-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f07c3-109">Property name</span></span>  | <span data-ttu-id="f07c3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f07c3-110">Type</span></span>    | <span data-ttu-id="f07c3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f07c3-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="f07c3-112">**format**</span><span class="sxs-lookup"><span data-stu-id="f07c3-112">**format**</span></span>     | <span data-ttu-id="f07c3-113">строка</span><span class="sxs-lookup"><span data-stu-id="f07c3-113">string</span></span>  | <span data-ttu-id="f07c3-114">Для типов выходных данных `dateTime` это свойство указывает формат значения.</span><span class="sxs-lookup"><span data-stu-id="f07c3-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="f07c3-115">Должно иметь тип `dateOnly` или `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="f07c3-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="f07c3-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="f07c3-116">**formula**</span></span>    | <span data-ttu-id="f07c3-117">строка</span><span class="sxs-lookup"><span data-stu-id="f07c3-117">string</span></span>  | <span data-ttu-id="f07c3-118">Формула, используемая для вычисления значения для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="f07c3-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="f07c3-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="f07c3-119">**outputType**</span></span> | <span data-ttu-id="f07c3-120">строка</span><span class="sxs-lookup"><span data-stu-id="f07c3-120">string</span></span>  | <span data-ttu-id="f07c3-121">Тип выходных данных, используемый для форматирования значений в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="f07c3-121">The output type used to format values in this column.</span></span> <span data-ttu-id="f07c3-122">Должно иметь один из типов `boolean`, `currency`, `dateTime`, `number` или `text`.</span><span class="sxs-lookup"><span data-stu-id="f07c3-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="f07c3-123">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="f07c3-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="f07c3-124">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="f07c3-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CalculatedColumn"
} -->
