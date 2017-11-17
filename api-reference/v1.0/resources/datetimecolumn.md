---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: dateTimeColumn
ms.openlocfilehash: ce5f06b6e0d88324813372c2431b62e6b9105bcb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="35b59-102">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="35b59-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="35b59-103">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columnDefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="35b59-103">The **dateTimeColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35b59-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="35b59-104">JSON representation</span></span>

<span data-ttu-id="35b59-105">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35b59-105">Here is a JSON representation of a **drive** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="35b59-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="35b59-106">Properties</span></span>

| <span data-ttu-id="35b59-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="35b59-107">Property name</span></span>      | <span data-ttu-id="35b59-108">Тип</span><span class="sxs-lookup"><span data-stu-id="35b59-108">Type</span></span>               | <span data-ttu-id="35b59-109">Описание</span><span class="sxs-lookup"><span data-stu-id="35b59-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="35b59-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="35b59-110">**displayAs**</span></span>      | <span data-ttu-id="35b59-111">строка</span><span class="sxs-lookup"><span data-stu-id="35b59-111">string</span></span>             | <span data-ttu-id="35b59-112">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="35b59-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="35b59-113">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="35b59-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="35b59-114">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="35b59-114">Read below for more details.</span></span> <span data-ttu-id="35b59-115">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="35b59-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="35b59-116">**format**</span><span class="sxs-lookup"><span data-stu-id="35b59-116">**format**</span></span>         | <span data-ttu-id="35b59-117">строка</span><span class="sxs-lookup"><span data-stu-id="35b59-117">string</span></span>             | <span data-ttu-id="35b59-118">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="35b59-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="35b59-119">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="35b59-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="35b59-120">Значения DisplayAs</span><span class="sxs-lookup"><span data-stu-id="35b59-120">DisplayAs values</span></span>

| <span data-ttu-id="35b59-121">Значение</span><span class="sxs-lookup"><span data-stu-id="35b59-121">Value</span></span>        | <span data-ttu-id="35b59-122">Описание</span><span class="sxs-lookup"><span data-stu-id="35b59-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="35b59-123">**default**</span><span class="sxs-lookup"><span data-stu-id="35b59-123">**Default**</span></span>  | <span data-ttu-id="35b59-124">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="35b59-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="35b59-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="35b59-125">**friendly**</span></span> | <span data-ttu-id="35b59-126">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="35b59-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="35b59-127">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="35b59-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="35b59-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="35b59-128">**Standard**</span></span> | <span data-ttu-id="35b59-129">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="35b59-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="35b59-130">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="35b59-130">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
