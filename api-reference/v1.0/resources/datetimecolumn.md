---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: ba650ccbe307ba286cf2182bda35a21f3c675114
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480175"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="236a8-102">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="236a8-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="236a8-103">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="236a8-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="236a8-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="236a8-104">JSON representation</span></span>

<span data-ttu-id="236a8-105">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="236a8-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="236a8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="236a8-106">Properties</span></span>

| <span data-ttu-id="236a8-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="236a8-107">Property name</span></span>      | <span data-ttu-id="236a8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="236a8-108">Type</span></span>               | <span data-ttu-id="236a8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="236a8-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="236a8-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="236a8-110">**displayAs**</span></span>      | <span data-ttu-id="236a8-111">string</span><span class="sxs-lookup"><span data-stu-id="236a8-111">string</span></span>             | <span data-ttu-id="236a8-112">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="236a8-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="236a8-113">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="236a8-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="236a8-114">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="236a8-114">See below for more details.</span></span> <span data-ttu-id="236a8-115">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="236a8-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="236a8-116">**format**</span><span class="sxs-lookup"><span data-stu-id="236a8-116">**format**</span></span>         | <span data-ttu-id="236a8-117">string</span><span class="sxs-lookup"><span data-stu-id="236a8-117">string</span></span>             | <span data-ttu-id="236a8-118">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="236a8-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="236a8-119">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="236a8-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="236a8-120">Параметры DisplayAs</span><span class="sxs-lookup"><span data-stu-id="236a8-120">DisplayAs options</span></span>

| <span data-ttu-id="236a8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="236a8-121">Value</span></span>        | <span data-ttu-id="236a8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="236a8-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="236a8-123">**default**</span><span class="sxs-lookup"><span data-stu-id="236a8-123">**default**</span></span>  | <span data-ttu-id="236a8-124">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="236a8-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="236a8-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="236a8-125">**friendly**</span></span> | <span data-ttu-id="236a8-126">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="236a8-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="236a8-127">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="236a8-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="236a8-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="236a8-128">**standard**</span></span> | <span data-ttu-id="236a8-129">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="236a8-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="236a8-130">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="236a8-130">"5/10/2017 3:20 PM")</span></span>


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
