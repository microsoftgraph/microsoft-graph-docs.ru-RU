---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: defaultColumnValue
localization_priority: Normal
ms.openlocfilehash: 6ceca45d09654771f161db63707682a4558b0d29
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815549"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="2aff3-102">Тип ресурса defaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="2aff3-102">DefaultColumnValue resource type</span></span>

> <span data-ttu-id="2aff3-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2aff3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2aff3-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2aff3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2aff3-105">Ресурс **defaultColumnValue** в ресурсе [columnDefinition](columndefinition.md) указывает значение, используемое по умолчанию, для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="2aff3-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="2aff3-106">Значение, используемое по умолчанию, можно указать либо непосредственно, либо в виде формулы.</span><span class="sxs-lookup"><span data-stu-id="2aff3-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2aff3-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2aff3-107">JSON representation</span></span>

<span data-ttu-id="2aff3-108">Ниже показано представление ресурса **defaultColumnValue** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2aff3-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="2aff3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2aff3-109">Properties</span></span>

| <span data-ttu-id="2aff3-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2aff3-110">Property name</span></span> | <span data-ttu-id="2aff3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2aff3-111">Type</span></span>   | <span data-ttu-id="2aff3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2aff3-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2aff3-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="2aff3-113">**formula**</span></span>   | <span data-ttu-id="2aff3-114">строка</span><span class="sxs-lookup"><span data-stu-id="2aff3-114">string</span></span> | <span data-ttu-id="2aff3-115">Формула, используемая для вычисления значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="2aff3-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="2aff3-116">**value**</span><span class="sxs-lookup"><span data-stu-id="2aff3-116">**value**</span></span>     | <span data-ttu-id="2aff3-117">строка</span><span class="sxs-lookup"><span data-stu-id="2aff3-117">string</span></span> | <span data-ttu-id="2aff3-118">Непосредственное значение, которое необходимо применять в качестве значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="2aff3-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="2aff3-119">Одновременно можно указать только одну **формулу** или одно **значение**.</span><span class="sxs-lookup"><span data-stu-id="2aff3-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="2aff3-120">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="2aff3-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="2aff3-121">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="2aff3-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
