---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
ms.openlocfilehash: e49b749adeaf7b04f9324fe00f9c73bf61f8b2dc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518683"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="0111e-102">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="0111e-102">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0111e-103">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="0111e-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0111e-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0111e-104">JSON representation</span></span>

<span data-ttu-id="0111e-105">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0111e-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="0111e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0111e-106">Properties</span></span>

| <span data-ttu-id="0111e-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="0111e-107">Property name</span></span>      | <span data-ttu-id="0111e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0111e-108">Type</span></span>               | <span data-ttu-id="0111e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0111e-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="0111e-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="0111e-110">**displayAs**</span></span>      | <span data-ttu-id="0111e-111">string</span><span class="sxs-lookup"><span data-stu-id="0111e-111">string</span></span>             | <span data-ttu-id="0111e-112">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="0111e-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="0111e-113">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="0111e-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="0111e-114">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="0111e-114">See below for more details.</span></span> <span data-ttu-id="0111e-115">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="0111e-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="0111e-116">**format**</span><span class="sxs-lookup"><span data-stu-id="0111e-116">**format**</span></span>         | <span data-ttu-id="0111e-117">string</span><span class="sxs-lookup"><span data-stu-id="0111e-117">string</span></span>             | <span data-ttu-id="0111e-118">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="0111e-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="0111e-119">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="0111e-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="0111e-120">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="0111e-120">DisplayAs values</span></span>

| <span data-ttu-id="0111e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0111e-121">Value</span></span>        | <span data-ttu-id="0111e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0111e-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="0111e-123">**default**</span><span class="sxs-lookup"><span data-stu-id="0111e-123">**default**</span></span>  | <span data-ttu-id="0111e-124">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="0111e-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="0111e-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="0111e-125">**friendly**</span></span> | <span data-ttu-id="0111e-126">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="0111e-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="0111e-127">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="0111e-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="0111e-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="0111e-128">**standard**</span></span> | <span data-ttu-id="0111e-129">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="0111e-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="0111e-130">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="0111e-130">"5/10/2017 3:20 PM")</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
