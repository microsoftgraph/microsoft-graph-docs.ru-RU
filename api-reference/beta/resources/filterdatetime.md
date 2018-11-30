---
title: Тип ресурса FilterDatetime
description: Представляет способ фильтрации даты при фильтрации по значениям.
ms.openlocfilehash: d3cb0df48a1116a64a72413aa64cabdec46da6d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079003"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="e56b3-103">Тип ресурса FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="e56b3-103">FilterDatetime resource type</span></span>

> <span data-ttu-id="e56b3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e56b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e56b3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e56b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e56b3-106">Представляет способ фильтрации даты при фильтрации по значениям.</span><span class="sxs-lookup"><span data-stu-id="e56b3-106">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="e56b3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e56b3-107">Properties</span></span>
| <span data-ttu-id="e56b3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e56b3-108">Property</span></span>     | <span data-ttu-id="e56b3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e56b3-109">Type</span></span>   |<span data-ttu-id="e56b3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e56b3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e56b3-111">дата</span><span class="sxs-lookup"><span data-stu-id="e56b3-111">date</span></span>|<span data-ttu-id="e56b3-112">строка</span><span class="sxs-lookup"><span data-stu-id="e56b3-112">string</span></span>|<span data-ttu-id="e56b3-113">Дата в формате ISO8601, используемая для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="e56b3-113">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="e56b3-114">specificity</span><span class="sxs-lookup"><span data-stu-id="e56b3-114">specificity</span></span>|<span data-ttu-id="e56b3-115">string</span><span class="sxs-lookup"><span data-stu-id="e56b3-115">string</span></span>|<span data-ttu-id="e56b3-p102">Точность, с которой производится фильтрация данных на основе даты. Например, если указана дата 2005-04-02, а для свойства specificity задано значение month, после фильтрации останутся все строки, датированные апрелем 2009 г. Возможные значения: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="e56b3-p102">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e56b3-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e56b3-119">Relationships</span></span>
<span data-ttu-id="e56b3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e56b3-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e56b3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e56b3-121">JSON representation</span></span>

<span data-ttu-id="e56b3-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e56b3-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->