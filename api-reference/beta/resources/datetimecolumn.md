---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
ms.openlocfilehash: b80e4a2e156baae4fbd8f3b559f061c50b45505f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340981"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="e13a2-102">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="e13a2-102">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e13a2-103">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="e13a2-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e13a2-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e13a2-104">JSON representation</span></span>

<span data-ttu-id="e13a2-105">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e13a2-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="e13a2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e13a2-106">Properties</span></span>

| <span data-ttu-id="e13a2-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="e13a2-107">Property name</span></span>      | <span data-ttu-id="e13a2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e13a2-108">Type</span></span>               | <span data-ttu-id="e13a2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e13a2-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="e13a2-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="e13a2-110">**displayAs**</span></span>      | <span data-ttu-id="e13a2-111">string</span><span class="sxs-lookup"><span data-stu-id="e13a2-111">string</span></span>             | <span data-ttu-id="e13a2-112">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="e13a2-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="e13a2-113">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="e13a2-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="e13a2-114">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="e13a2-114">See below for more details.</span></span> <span data-ttu-id="e13a2-115">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="e13a2-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="e13a2-116">**format**</span><span class="sxs-lookup"><span data-stu-id="e13a2-116">**format**</span></span>         | <span data-ttu-id="e13a2-117">строка</span><span class="sxs-lookup"><span data-stu-id="e13a2-117">string</span></span>             | <span data-ttu-id="e13a2-118">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="e13a2-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="e13a2-119">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="e13a2-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="e13a2-120">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="e13a2-120">DisplayAs values</span></span>

| <span data-ttu-id="e13a2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e13a2-121">Value</span></span>        | <span data-ttu-id="e13a2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e13a2-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="e13a2-123">**default**</span><span class="sxs-lookup"><span data-stu-id="e13a2-123">**default**</span></span>  | <span data-ttu-id="e13a2-124">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="e13a2-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="e13a2-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="e13a2-125">**friendly**</span></span> | <span data-ttu-id="e13a2-126">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="e13a2-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="e13a2-127">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="e13a2-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="e13a2-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="e13a2-128">**standard**</span></span> | <span data-ttu-id="e13a2-129">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="e13a2-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="e13a2-130">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="e13a2-130">"5/10/2017 3:20 PM")</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn",
  "suppressions": []
}
-->
