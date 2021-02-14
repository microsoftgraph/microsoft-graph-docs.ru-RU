---
author: daspek
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
description: Ресурс defaultColumnValue в ресурсе columnDefinition указывает значение, используемое по умолчанию, для этого столбца.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 881927bdbd53936d7780fa7517b2d2428c524e78
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239641"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="f8ebb-103">Тип ресурса defaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="f8ebb-103">DefaultColumnValue resource type</span></span>

<span data-ttu-id="f8ebb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8ebb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8ebb-105">Ресурс **defaultColumnValue** в ресурсе [columnDefinition](columndefinition.md) указывает значение, используемое по умолчанию, для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="f8ebb-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="f8ebb-106">Значение, используемое по умолчанию, можно указать либо непосредственно, либо в виде формулы.</span><span class="sxs-lookup"><span data-stu-id="f8ebb-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8ebb-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f8ebb-107">JSON representation</span></span>

<span data-ttu-id="f8ebb-108">Ниже показано представление ресурса **defaultColumnValue** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8ebb-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="f8ebb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8ebb-109">Properties</span></span>

| <span data-ttu-id="f8ebb-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="f8ebb-110">Property name</span></span> | <span data-ttu-id="f8ebb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f8ebb-111">Type</span></span>   | <span data-ttu-id="f8ebb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f8ebb-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f8ebb-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="f8ebb-113">**formula**</span></span>   | <span data-ttu-id="f8ebb-114">string</span><span class="sxs-lookup"><span data-stu-id="f8ebb-114">string</span></span> | <span data-ttu-id="f8ebb-115">Формула, используемая для вычисления значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="f8ebb-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="f8ebb-116">**value**</span><span class="sxs-lookup"><span data-stu-id="f8ebb-116">**value**</span></span>     | <span data-ttu-id="f8ebb-117">string</span><span class="sxs-lookup"><span data-stu-id="f8ebb-117">string</span></span> | <span data-ttu-id="f8ebb-118">Непосредственное значение, которое необходимо применять в качестве значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="f8ebb-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="f8ebb-119">Одновременно можно указать только одну **формулу** или одно **значение**.</span><span class="sxs-lookup"><span data-stu-id="f8ebb-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="f8ebb-120">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="f8ebb-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="f8ebb-121">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="f8ebb-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->

