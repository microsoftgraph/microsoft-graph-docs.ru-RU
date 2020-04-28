---
author: JeremyKelley
description: Ресурс calculatedColumn в ресурсе columnDefinition указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.
ms.date: 09/11/2017
title: calculatedColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c9bd8963ed847e60bb5b71abfd100cd372dd1dc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507854"
---
# <a name="calculatedcolumn-resource-type"></a><span data-ttu-id="24b13-103">Тип ресурса calculatedColumn</span><span class="sxs-lookup"><span data-stu-id="24b13-103">CalculatedColumn resource type</span></span>

<span data-ttu-id="24b13-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24b13-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24b13-105">Ресурс **calculatedColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что данные столбца вычисляются на основании значений в других столбцах на сайте.</span><span class="sxs-lookup"><span data-stu-id="24b13-105">The **calculatedColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's data is calculated based on other columns in the site.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24b13-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="24b13-106">JSON representation</span></span>

<span data-ttu-id="24b13-107">Ниже показано представление ресурса **calculatedColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24b13-107">Here is a JSON representation of a **calculatedColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.calculatedColumn" } -->

```json
{
  "format": "dateOnly | dateTime",
  "formula": "=[Column1]+[Column2]+[Column3]",
  "outputType": "boolean | currency | dateTime | number | text",
}
```

## <a name="properties"></a><span data-ttu-id="24b13-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="24b13-108">Properties</span></span>

| <span data-ttu-id="24b13-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="24b13-109">Property name</span></span>  | <span data-ttu-id="24b13-110">Тип</span><span class="sxs-lookup"><span data-stu-id="24b13-110">Type</span></span>    | <span data-ttu-id="24b13-111">Описание</span><span class="sxs-lookup"><span data-stu-id="24b13-111">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="24b13-112">**format**</span><span class="sxs-lookup"><span data-stu-id="24b13-112">**format**</span></span>     | <span data-ttu-id="24b13-113">строка</span><span class="sxs-lookup"><span data-stu-id="24b13-113">string</span></span>  | <span data-ttu-id="24b13-114">Для типов выходных данных `dateTime` это свойство указывает формат значения.</span><span class="sxs-lookup"><span data-stu-id="24b13-114">For `dateTime` output types, the format of the value.</span></span> <span data-ttu-id="24b13-115">Должно иметь тип `dateOnly` или `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="24b13-115">Must be one of `dateOnly` or `dateTime`.</span></span>
| <span data-ttu-id="24b13-116">**formula**</span><span class="sxs-lookup"><span data-stu-id="24b13-116">**formula**</span></span>    | <span data-ttu-id="24b13-117">string</span><span class="sxs-lookup"><span data-stu-id="24b13-117">string</span></span>  | <span data-ttu-id="24b13-118">Формула, используемая для вычисления значения для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="24b13-118">The formula used to compute the value for this column.</span></span>
| <span data-ttu-id="24b13-119">**outputType**</span><span class="sxs-lookup"><span data-stu-id="24b13-119">**outputType**</span></span> | <span data-ttu-id="24b13-120">string</span><span class="sxs-lookup"><span data-stu-id="24b13-120">string</span></span>  | <span data-ttu-id="24b13-121">Тип выходных данных, используемый для форматирования значений в этом столбце.</span><span class="sxs-lookup"><span data-stu-id="24b13-121">The output type used to format values in this column.</span></span> <span data-ttu-id="24b13-122">Должно иметь один из типов `boolean`, `currency`, `dateTime`, `number` или `text`.</span><span class="sxs-lookup"><span data-stu-id="24b13-122">Must be one of `boolean`, `currency`, `dateTime`, `number`, or `text`.</span></span>

<span data-ttu-id="24b13-123">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="24b13-123">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="24b13-124">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="24b13-124">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

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
