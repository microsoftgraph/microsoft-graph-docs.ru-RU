---
author: JeremyKelley
description: Ресурс dateTimeColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой даты или время.
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7de33a9c1f4d6aa3d47495afdbfdb201e74bf11e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050000"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="5398f-103">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="5398f-103">DateTimeColumn resource type</span></span>

<span data-ttu-id="5398f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5398f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5398f-105">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="5398f-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5398f-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5398f-106">JSON representation</span></span>

<span data-ttu-id="5398f-107">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5398f-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="5398f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5398f-108">Properties</span></span>

| <span data-ttu-id="5398f-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5398f-109">Property name</span></span>      | <span data-ttu-id="5398f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5398f-110">Type</span></span>               | <span data-ttu-id="5398f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5398f-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="5398f-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="5398f-112">**displayAs**</span></span>      | <span data-ttu-id="5398f-113">string</span><span class="sxs-lookup"><span data-stu-id="5398f-113">string</span></span>             | <span data-ttu-id="5398f-114">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="5398f-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="5398f-115">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="5398f-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="5398f-116">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="5398f-116">See below for more details.</span></span> <span data-ttu-id="5398f-117">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="5398f-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="5398f-118">**format**</span><span class="sxs-lookup"><span data-stu-id="5398f-118">**format**</span></span>         | <span data-ttu-id="5398f-119">строка</span><span class="sxs-lookup"><span data-stu-id="5398f-119">string</span></span>             | <span data-ttu-id="5398f-120">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="5398f-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="5398f-121">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="5398f-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="5398f-122">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="5398f-122">DisplayAs values</span></span>

| <span data-ttu-id="5398f-123">Значение</span><span class="sxs-lookup"><span data-stu-id="5398f-123">Value</span></span>        | <span data-ttu-id="5398f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5398f-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="5398f-125">**default**</span><span class="sxs-lookup"><span data-stu-id="5398f-125">**default**</span></span>  | <span data-ttu-id="5398f-126">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="5398f-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="5398f-127">**friendly**</span><span class="sxs-lookup"><span data-stu-id="5398f-127">**friendly**</span></span> | <span data-ttu-id="5398f-128">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="5398f-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="5398f-129">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="5398f-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="5398f-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="5398f-130">**standard**</span></span> | <span data-ttu-id="5398f-131">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="5398f-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="5398f-132">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="5398f-132">"5/10/2017 3:20 PM")</span></span>


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


