---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
description: Ресурс dateTimeColumn в ресурсе columnDefinition указывает, что значения столбца представляют собой даты или время.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4c3f5fa00af8b04753f6581120760b5a57a9e08a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531723"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="9bc61-103">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="9bc61-103">DateTimeColumn resource type</span></span>

<span data-ttu-id="9bc61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bc61-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9bc61-105">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="9bc61-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bc61-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9bc61-106">JSON representation</span></span>

<span data-ttu-id="9bc61-107">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bc61-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="9bc61-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bc61-108">Properties</span></span>

| <span data-ttu-id="9bc61-109">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="9bc61-109">Property name</span></span>      | <span data-ttu-id="9bc61-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9bc61-110">Type</span></span>               | <span data-ttu-id="9bc61-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9bc61-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="9bc61-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="9bc61-112">**displayAs**</span></span>      | <span data-ttu-id="9bc61-113">string</span><span class="sxs-lookup"><span data-stu-id="9bc61-113">string</span></span>             | <span data-ttu-id="9bc61-114">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="9bc61-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="9bc61-115">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="9bc61-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="9bc61-116">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="9bc61-116">See below for more details.</span></span> <span data-ttu-id="9bc61-117">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="9bc61-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="9bc61-118">**format**</span><span class="sxs-lookup"><span data-stu-id="9bc61-118">**format**</span></span>         | <span data-ttu-id="9bc61-119">строка</span><span class="sxs-lookup"><span data-stu-id="9bc61-119">string</span></span>             | <span data-ttu-id="9bc61-120">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="9bc61-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="9bc61-121">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="9bc61-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="9bc61-122">Параметры DisplayAs</span><span class="sxs-lookup"><span data-stu-id="9bc61-122">DisplayAs options</span></span>

| <span data-ttu-id="9bc61-123">Значение</span><span class="sxs-lookup"><span data-stu-id="9bc61-123">Value</span></span>        | <span data-ttu-id="9bc61-124">Описание</span><span class="sxs-lookup"><span data-stu-id="9bc61-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="9bc61-125">**default**</span><span class="sxs-lookup"><span data-stu-id="9bc61-125">**default**</span></span>  | <span data-ttu-id="9bc61-126">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="9bc61-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="9bc61-127">**friendly**</span><span class="sxs-lookup"><span data-stu-id="9bc61-127">**friendly**</span></span> | <span data-ttu-id="9bc61-128">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="9bc61-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="9bc61-129">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="9bc61-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="9bc61-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="9bc61-130">**standard**</span></span> | <span data-ttu-id="9bc61-131">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="9bc61-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="9bc61-132">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="9bc61-132">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(default,friendly,standard) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table"
  ],
  "tocPath": "Resources/DateTimeColumn"
} -->
