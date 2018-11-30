---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: defaultColumnValue
ms.openlocfilehash: 73761e224a59b3a9a4206d5e1cfb058294b7f53b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="48336-102">Тип ресурса defaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="48336-102">DefaultColumnValue resource type</span></span>

<span data-ttu-id="48336-103">Ресурс **defaultColumnValue** в ресурсе [columnDefinition](columnDefinition.md) указывает значение, используемое по умолчанию, для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="48336-103">The **defaultColumnValue** on a [columnDefinition](columnDefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="48336-104">Значение, используемое по умолчанию, можно указать либо непосредственно, либо в виде формулы.</span><span class="sxs-lookup"><span data-stu-id="48336-104">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="48336-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="48336-105">JSON representation</span></span>

<span data-ttu-id="48336-106">Ниже показано представление ресурса **defaultColumnValue** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="48336-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="48336-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="48336-107">Properties</span></span>

| <span data-ttu-id="48336-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="48336-108">Property name</span></span> | <span data-ttu-id="48336-109">Тип</span><span class="sxs-lookup"><span data-stu-id="48336-109">Type</span></span>   | <span data-ttu-id="48336-110">Описание</span><span class="sxs-lookup"><span data-stu-id="48336-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="48336-111">**formula**</span><span class="sxs-lookup"><span data-stu-id="48336-111">**formula**</span></span>   | <span data-ttu-id="48336-112">строка</span><span class="sxs-lookup"><span data-stu-id="48336-112">string</span></span> | <span data-ttu-id="48336-113">Формула, которая применяется для вычисления значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="48336-113">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="48336-114">**value**</span><span class="sxs-lookup"><span data-stu-id="48336-114">**value**</span></span>     | <span data-ttu-id="48336-115">строка</span><span class="sxs-lookup"><span data-stu-id="48336-115">string</span></span> | <span data-ttu-id="48336-116">Непосредственное значение, которое необходимо применять в качестве значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="48336-116">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="48336-117">Одновременно можно указать только одну **формулу** или одно **значение**.</span><span class="sxs-lookup"><span data-stu-id="48336-117">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="48336-118">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="48336-118">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="48336-119">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="48336-119">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
