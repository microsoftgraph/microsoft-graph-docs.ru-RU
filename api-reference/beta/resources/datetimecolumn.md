---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
ms.openlocfilehash: da8fe44e377a071ee3f20b82f7190b690dcfd6b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535293"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="8d816-102">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="8d816-102">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d816-103">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="8d816-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d816-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8d816-104">JSON representation</span></span>

<span data-ttu-id="8d816-105">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d816-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="8d816-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d816-106">Properties</span></span>

| <span data-ttu-id="8d816-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="8d816-107">Property name</span></span>      | <span data-ttu-id="8d816-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8d816-108">Type</span></span>               | <span data-ttu-id="8d816-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8d816-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="8d816-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="8d816-110">**displayAs**</span></span>      | <span data-ttu-id="8d816-111">string</span><span class="sxs-lookup"><span data-stu-id="8d816-111">string</span></span>             | <span data-ttu-id="8d816-112">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="8d816-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="8d816-113">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="8d816-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="8d816-114">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="8d816-114">See below for more details.</span></span> <span data-ttu-id="8d816-115">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="8d816-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="8d816-116">**format**</span><span class="sxs-lookup"><span data-stu-id="8d816-116">**format**</span></span>         | <span data-ttu-id="8d816-117">строка</span><span class="sxs-lookup"><span data-stu-id="8d816-117">string</span></span>             | <span data-ttu-id="8d816-118">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="8d816-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="8d816-119">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="8d816-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="8d816-120">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="8d816-120">DisplayAs values</span></span>

| <span data-ttu-id="8d816-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8d816-121">Value</span></span>        | <span data-ttu-id="8d816-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8d816-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="8d816-123">**default**</span><span class="sxs-lookup"><span data-stu-id="8d816-123">**default**</span></span>  | <span data-ttu-id="8d816-124">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="8d816-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="8d816-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="8d816-125">**friendly**</span></span> | <span data-ttu-id="8d816-126">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="8d816-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="8d816-127">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="8d816-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="8d816-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="8d816-128">**standard**</span></span> | <span data-ttu-id="8d816-129">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="8d816-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="8d816-130">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="8d816-130">"5/10/2017 3:20 PM")</span></span>


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
