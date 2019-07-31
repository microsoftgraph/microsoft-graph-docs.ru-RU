---
author: daspek
description: Ресурс defaultColumnValue в ресурсе columnDefinition указывает значение, используемое по умолчанию, для этого столбца.
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9c59fd3303f014f8f9f78d8abc52b7f7ff59ade1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973155"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="60e57-103">Тип ресурса defaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="60e57-103">DefaultColumnValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60e57-104">Ресурс **defaultColumnValue** в ресурсе [columnDefinition](columndefinition.md) указывает значение, используемое по умолчанию, для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="60e57-104">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="60e57-105">Значение, используемое по умолчанию, можно указать либо непосредственно, либо в виде формулы.</span><span class="sxs-lookup"><span data-stu-id="60e57-105">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60e57-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="60e57-106">JSON representation</span></span>

<span data-ttu-id="60e57-107">Ниже показано представление ресурса **defaultColumnValue** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60e57-107">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="60e57-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="60e57-108">Properties</span></span>

| <span data-ttu-id="60e57-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="60e57-109">Property name</span></span> | <span data-ttu-id="60e57-110">Тип</span><span class="sxs-lookup"><span data-stu-id="60e57-110">Type</span></span>   | <span data-ttu-id="60e57-111">Описание</span><span class="sxs-lookup"><span data-stu-id="60e57-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="60e57-112">**formula**</span><span class="sxs-lookup"><span data-stu-id="60e57-112">**formula**</span></span>   | <span data-ttu-id="60e57-113">string</span><span class="sxs-lookup"><span data-stu-id="60e57-113">string</span></span> | <span data-ttu-id="60e57-114">Формула, используемая для вычисления значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="60e57-114">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="60e57-115">**value**</span><span class="sxs-lookup"><span data-stu-id="60e57-115">**value**</span></span>     | <span data-ttu-id="60e57-116">string</span><span class="sxs-lookup"><span data-stu-id="60e57-116">string</span></span> | <span data-ttu-id="60e57-117">Непосредственное значение, которое необходимо применять в качестве значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="60e57-117">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="60e57-118">Одновременно можно указать только одну **формулу** или одно **значение**.</span><span class="sxs-lookup"><span data-stu-id="60e57-118">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="60e57-119">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="60e57-119">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="60e57-120">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="60e57-120">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue",
  "suppressions": []
}
-->
