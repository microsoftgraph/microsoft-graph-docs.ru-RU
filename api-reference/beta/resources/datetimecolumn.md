---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: da8fe44e377a071ee3f20b82f7190b690dcfd6b2
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482170"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="155c7-102">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="155c7-102">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="155c7-103">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="155c7-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="155c7-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="155c7-104">JSON representation</span></span>

<span data-ttu-id="155c7-105">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="155c7-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="155c7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="155c7-106">Properties</span></span>

| <span data-ttu-id="155c7-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="155c7-107">Property name</span></span>      | <span data-ttu-id="155c7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="155c7-108">Type</span></span>               | <span data-ttu-id="155c7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="155c7-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="155c7-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="155c7-110">**displayAs**</span></span>      | <span data-ttu-id="155c7-111">string</span><span class="sxs-lookup"><span data-stu-id="155c7-111">string</span></span>             | <span data-ttu-id="155c7-112">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="155c7-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="155c7-113">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="155c7-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="155c7-114">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="155c7-114">See below for more details.</span></span> <span data-ttu-id="155c7-115">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="155c7-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="155c7-116">**format**</span><span class="sxs-lookup"><span data-stu-id="155c7-116">**format**</span></span>         | <span data-ttu-id="155c7-117">string</span><span class="sxs-lookup"><span data-stu-id="155c7-117">string</span></span>             | <span data-ttu-id="155c7-118">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="155c7-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="155c7-119">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="155c7-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="155c7-120">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="155c7-120">DisplayAs values</span></span>

| <span data-ttu-id="155c7-121">Значение</span><span class="sxs-lookup"><span data-stu-id="155c7-121">Value</span></span>        | <span data-ttu-id="155c7-122">Описание</span><span class="sxs-lookup"><span data-stu-id="155c7-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="155c7-123">**default**</span><span class="sxs-lookup"><span data-stu-id="155c7-123">**default**</span></span>  | <span data-ttu-id="155c7-124">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="155c7-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="155c7-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="155c7-125">**friendly**</span></span> | <span data-ttu-id="155c7-126">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="155c7-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="155c7-127">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="155c7-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="155c7-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="155c7-128">**standard**</span></span> | <span data-ttu-id="155c7-129">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="155c7-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="155c7-130">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="155c7-130">"5/10/2017 3:20 PM")</span></span>


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
