---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: dateTimeColumn
ms.openlocfilehash: 9854ad35c602ff474604f2ca88e7182c325e797d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075531"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="2865d-102">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="2865d-102">DateTimeColumn resource type</span></span>

> <span data-ttu-id="2865d-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2865d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2865d-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2865d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2865d-105">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="2865d-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2865d-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2865d-106">JSON representation</span></span>

<span data-ttu-id="2865d-107">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2865d-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="2865d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2865d-108">Properties</span></span>

| <span data-ttu-id="2865d-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="2865d-109">Property name</span></span>      | <span data-ttu-id="2865d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2865d-110">Type</span></span>               | <span data-ttu-id="2865d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2865d-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="2865d-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="2865d-112">**displayAs**</span></span>      | <span data-ttu-id="2865d-113">строка</span><span class="sxs-lookup"><span data-stu-id="2865d-113">string</span></span>             | <span data-ttu-id="2865d-114">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="2865d-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="2865d-115">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="2865d-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="2865d-116">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="2865d-116">See below for more details.</span></span> <span data-ttu-id="2865d-117">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="2865d-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="2865d-118">**format**</span><span class="sxs-lookup"><span data-stu-id="2865d-118">**format**</span></span>         | <span data-ttu-id="2865d-119">строка</span><span class="sxs-lookup"><span data-stu-id="2865d-119">string</span></span>             | <span data-ttu-id="2865d-120">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="2865d-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="2865d-121">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="2865d-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="2865d-122">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="2865d-122">DisplayAs values</span></span>

| <span data-ttu-id="2865d-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2865d-123">Value</span></span>        | <span data-ttu-id="2865d-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2865d-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="2865d-125">**default**</span><span class="sxs-lookup"><span data-stu-id="2865d-125">**default**</span></span>  | <span data-ttu-id="2865d-126">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="2865d-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="2865d-127">**friendly**</span><span class="sxs-lookup"><span data-stu-id="2865d-127">**friendly**</span></span> | <span data-ttu-id="2865d-128">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="2865d-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="2865d-129">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="2865d-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="2865d-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="2865d-130">**standard**</span></span> | <span data-ttu-id="2865d-131">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="2865d-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="2865d-132">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="2865d-132">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
