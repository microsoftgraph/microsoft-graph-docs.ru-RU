---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: dateTimeColumn
localization_priority: Normal
ms.openlocfilehash: ba650ccbe307ba286cf2182bda35a21f3c675114
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574766"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="6ef1f-102">Тип ресурса dateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="6ef1f-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="6ef1f-103">Ресурс **dateTimeColumn** в ресурсе [columnDefinition](columndefinition.md) указывает, что значения столбца представляют собой даты или время.</span><span class="sxs-lookup"><span data-stu-id="6ef1f-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ef1f-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6ef1f-104">JSON representation</span></span>

<span data-ttu-id="6ef1f-105">Ниже показано представление ресурса **dateTimeColumn** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ef1f-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="6ef1f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ef1f-106">Properties</span></span>

| <span data-ttu-id="6ef1f-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="6ef1f-107">Property name</span></span>      | <span data-ttu-id="6ef1f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6ef1f-108">Type</span></span>               | <span data-ttu-id="6ef1f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6ef1f-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="6ef1f-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="6ef1f-110">**displayAs**</span></span>      | <span data-ttu-id="6ef1f-111">string</span><span class="sxs-lookup"><span data-stu-id="6ef1f-111">string</span></span>             | <span data-ttu-id="6ef1f-112">Способ отображения значения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="6ef1f-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="6ef1f-113">Должно иметь один из типов `default`, `friendly` или `standard`.</span><span class="sxs-lookup"><span data-stu-id="6ef1f-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="6ef1f-114">Дополнительные сведения см. ниже.</span><span class="sxs-lookup"><span data-stu-id="6ef1f-114">See below for more details.</span></span> <span data-ttu-id="6ef1f-115">Если тип не указан, считается, что значение имеет тип `default`.</span><span class="sxs-lookup"><span data-stu-id="6ef1f-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="6ef1f-116">**format**</span><span class="sxs-lookup"><span data-stu-id="6ef1f-116">**format**</span></span>         | <span data-ttu-id="6ef1f-117">строка</span><span class="sxs-lookup"><span data-stu-id="6ef1f-117">string</span></span>             | <span data-ttu-id="6ef1f-118">Указывает способ представления значения: только в виде даты либо в виде даты и времени.</span><span class="sxs-lookup"><span data-stu-id="6ef1f-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="6ef1f-119">Должно иметь тип `dateOnly` или `dateTime`</span><span class="sxs-lookup"><span data-stu-id="6ef1f-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="6ef1f-120">Параметры DisplayAs</span><span class="sxs-lookup"><span data-stu-id="6ef1f-120">DisplayAs options</span></span>

| <span data-ttu-id="6ef1f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6ef1f-121">Value</span></span>        | <span data-ttu-id="6ef1f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6ef1f-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="6ef1f-123">**default**</span><span class="sxs-lookup"><span data-stu-id="6ef1f-123">**default**</span></span>  | <span data-ttu-id="6ef1f-124">Применение способа отображения, используемого по умолчанию, в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="6ef1f-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="6ef1f-125">**friendly**</span><span class="sxs-lookup"><span data-stu-id="6ef1f-125">**friendly**</span></span> | <span data-ttu-id="6ef1f-126">Использование понятного относительного представления (например,</span><span class="sxs-lookup"><span data-stu-id="6ef1f-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="6ef1f-127">"сегодня в 15:00")</span><span class="sxs-lookup"><span data-stu-id="6ef1f-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="6ef1f-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="6ef1f-128">**standard**</span></span> | <span data-ttu-id="6ef1f-129">Использование стандартного абсолютного представления (например,</span><span class="sxs-lookup"><span data-stu-id="6ef1f-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="6ef1f-130">"10.05.2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="6ef1f-130">"5/10/2017 3:20 PM")</span></span>


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
