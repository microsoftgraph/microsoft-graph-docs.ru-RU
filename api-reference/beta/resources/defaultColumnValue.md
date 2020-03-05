---
author: daspek
description: Ресурс defaultColumnValue в ресурсе columnDefinition указывает значение, используемое по умолчанию, для этого столбца.
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 57c66b627a61c59f78166bd8d6a14aef41cdd36d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507284"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="cd04a-103">Тип ресурса defaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="cd04a-103">DefaultColumnValue resource type</span></span>

<span data-ttu-id="cd04a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cd04a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd04a-105">Ресурс **defaultColumnValue** в ресурсе [columnDefinition](columndefinition.md) указывает значение, используемое по умолчанию, для этого столбца.</span><span class="sxs-lookup"><span data-stu-id="cd04a-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="cd04a-106">Значение, используемое по умолчанию, можно указать либо непосредственно, либо в виде формулы.</span><span class="sxs-lookup"><span data-stu-id="cd04a-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd04a-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cd04a-107">JSON representation</span></span>

<span data-ttu-id="cd04a-108">Ниже показано представление ресурса **defaultColumnValue** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd04a-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="cd04a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd04a-109">Properties</span></span>

| <span data-ttu-id="cd04a-110">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="cd04a-110">Property name</span></span> | <span data-ttu-id="cd04a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="cd04a-111">Type</span></span>   | <span data-ttu-id="cd04a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="cd04a-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="cd04a-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="cd04a-113">**formula**</span></span>   | <span data-ttu-id="cd04a-114">строка</span><span class="sxs-lookup"><span data-stu-id="cd04a-114">string</span></span> | <span data-ttu-id="cd04a-115">Формула, используемая для вычисления значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="cd04a-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="cd04a-116">**value**</span><span class="sxs-lookup"><span data-stu-id="cd04a-116">**value**</span></span>     | <span data-ttu-id="cd04a-117">string</span><span class="sxs-lookup"><span data-stu-id="cd04a-117">string</span></span> | <span data-ttu-id="cd04a-118">Непосредственное значение, которое необходимо применять в качестве значения, используемого по умолчанию, для данного столбца.</span><span class="sxs-lookup"><span data-stu-id="cd04a-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="cd04a-119">Одновременно можно указать только одну **формулу** или одно **значение**.</span><span class="sxs-lookup"><span data-stu-id="cd04a-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="cd04a-120">В формулах SharePoint используется синтаксис, похожий на синтаксис формул в Excel.</span><span class="sxs-lookup"><span data-stu-id="cd04a-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="cd04a-121">Дополнительные сведения см. в статье [Примеры часто используемых формул в списках SharePoint][SPFormulas].</span><span class="sxs-lookup"><span data-stu-id="cd04a-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

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
