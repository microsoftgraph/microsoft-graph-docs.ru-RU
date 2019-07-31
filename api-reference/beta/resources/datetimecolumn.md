---
author: JeremyKelley
description: Ресурс dateTimeColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой даты или время.
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e0e69e4019530031966cde9f782c2f017ba976fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973890"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="2dc7e-103">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="2dc7e-103">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dc7e-104">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="2dc7e-104">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dc7e-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2dc7e-105">JSON representation</span></span>

<span data-ttu-id="2dc7e-106">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dc7e-106">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="2dc7e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dc7e-107">Properties</span></span>

| <span data-ttu-id="2dc7e-108">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2dc7e-108">Property name</span></span>      | <span data-ttu-id="2dc7e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2dc7e-109">Type</span></span>               | <span data-ttu-id="2dc7e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc7e-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="2dc7e-111">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="2dc7e-111">**displayAs**</span></span>      | <span data-ttu-id="2dc7e-112">string</span><span class="sxs-lookup"><span data-stu-id="2dc7e-112">string</span></span>             | <span data-ttu-id="2dc7e-113">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="2dc7e-113">How the value should be presented in the UX.</span></span> <span data-ttu-id="2dc7e-114">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="2dc7e-114">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="2dc7e-115">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="2dc7e-115">See below for more details.</span></span> <span data-ttu-id="2dc7e-116">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="2dc7e-116">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="2dc7e-117">**format**</span><span class="sxs-lookup"><span data-stu-id="2dc7e-117">**format**</span></span>         | <span data-ttu-id="2dc7e-118">строка</span><span class="sxs-lookup"><span data-stu-id="2dc7e-118">string</span></span>             | <span data-ttu-id="2dc7e-119">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="2dc7e-119">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="2dc7e-120">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="2dc7e-120">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="2dc7e-121">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="2dc7e-121">DisplayAs values</span></span>

| <span data-ttu-id="2dc7e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2dc7e-122">Value</span></span>        | <span data-ttu-id="2dc7e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2dc7e-123">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="2dc7e-124">**default**</span><span class="sxs-lookup"><span data-stu-id="2dc7e-124">**default**</span></span>  | <span data-ttu-id="2dc7e-125">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="2dc7e-125">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="2dc7e-126">**friendly**</span><span class="sxs-lookup"><span data-stu-id="2dc7e-126">**friendly**</span></span> | <span data-ttu-id="2dc7e-127">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="2dc7e-127">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="2dc7e-128">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="2dc7e-128">"today at 3:00 PM")</span></span>
| <span data-ttu-id="2dc7e-129">**standard**</span><span class="sxs-lookup"><span data-stu-id="2dc7e-129">**standard**</span></span> | <span data-ttu-id="2dc7e-130">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="2dc7e-130">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="2dc7e-131">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="2dc7e-131">"5/10/2017 3:20 PM")</span></span>


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
