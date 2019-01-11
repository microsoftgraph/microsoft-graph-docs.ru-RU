---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: defaultColumnValue
localization_priority: Normal
ms.openlocfilehash: 400fc25bf38f12db2be8cef21ddc351316d1265b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810593"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="7b909-102">Тип ресурса defaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="7b909-102">DefaultColumnValue resource type</span></span>

<span data-ttu-id="7b909-103">Ресурс **defaultColumnValue** в ресурсе [columnDefinition](columndefinition.md) указывает значение, используемое по умолчанию, для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="7b909-103">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="7b909-104">Значение, используемое по умолчанию, можно указать либо непосредственно, либо в виде формулы.</span><span class="sxs-lookup"><span data-stu-id="7b909-104">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b909-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7b909-105">JSON representation</span></span>

<span data-ttu-id="7b909-106">Ниже показано представление ресурса **defaultColumnValue** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b909-106">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="7b909-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b909-107">Properties</span></span>

| <span data-ttu-id="7b909-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7b909-108">Property name</span></span> | <span data-ttu-id="7b909-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7b909-109">Type</span></span>   | <span data-ttu-id="7b909-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b909-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="7b909-111">**formula**</span><span class="sxs-lookup"><span data-stu-id="7b909-111">**formula**</span></span>   | <span data-ttu-id="7b909-112">string</span><span class="sxs-lookup"><span data-stu-id="7b909-112">string</span></span> | <span data-ttu-id="7b909-113">Формула, используемая для вычисления значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="7b909-113">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="7b909-114">**value**</span><span class="sxs-lookup"><span data-stu-id="7b909-114">**value**</span></span>     | <span data-ttu-id="7b909-115">string</span><span class="sxs-lookup"><span data-stu-id="7b909-115">string</span></span> | <span data-ttu-id="7b909-116">Непосредственное значение, которое необходимо применять в качестве значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="7b909-116">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="7b909-117">Одновременно можно указать только одну **формулу** или одно **значение**.</span><span class="sxs-lookup"><span data-stu-id="7b909-117">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="7b909-118">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="7b909-118">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="7b909-119">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="7b909-119">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
