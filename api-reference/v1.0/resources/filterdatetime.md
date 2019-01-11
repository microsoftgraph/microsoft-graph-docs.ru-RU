---
title: Тип ресурса FilterDatetime
description: Представляет способ фильтрации даты при фильтрации по значениям.
localization_priority: Normal
ms.openlocfilehash: 26d42b45a2e9b9cdd279f33330a877a64ea1c8d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840364"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="aefe6-103">Тип ресурса FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="aefe6-103">FilterDatetime resource type</span></span>

<span data-ttu-id="aefe6-104">Представляет способ фильтрации даты при фильтрации по значениям.</span><span class="sxs-lookup"><span data-stu-id="aefe6-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="aefe6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="aefe6-105">Properties</span></span>
| <span data-ttu-id="aefe6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="aefe6-106">Property</span></span>     | <span data-ttu-id="aefe6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="aefe6-107">Type</span></span>   |<span data-ttu-id="aefe6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="aefe6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aefe6-109">дата</span><span class="sxs-lookup"><span data-stu-id="aefe6-109">date</span></span>|<span data-ttu-id="aefe6-110">строка</span><span class="sxs-lookup"><span data-stu-id="aefe6-110">string</span></span>|<span data-ttu-id="aefe6-111">Дата в формате ISO8601, используемая для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="aefe6-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="aefe6-112">specificity</span><span class="sxs-lookup"><span data-stu-id="aefe6-112">specificity</span></span>|<span data-ttu-id="aefe6-113">string</span><span class="sxs-lookup"><span data-stu-id="aefe6-113">string</span></span>|<span data-ttu-id="aefe6-114">Каким образом определенные даты можно использовать для хранения данных.</span><span class="sxs-lookup"><span data-stu-id="aefe6-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="aefe6-115">Например если дата 2005-04-02 и specifity задано значение «месяц», операцию фильтра будет сохранено все строки с датой в месяц апреля 2009 г..</span><span class="sxs-lookup"><span data-stu-id="aefe6-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="aefe6-116">Возможные значения: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="aefe6-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aefe6-117">Связи</span><span class="sxs-lookup"><span data-stu-id="aefe6-117">Relationships</span></span>
<span data-ttu-id="aefe6-118">Нет</span><span class="sxs-lookup"><span data-stu-id="aefe6-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="aefe6-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aefe6-119">JSON representation</span></span>

<span data-ttu-id="aefe6-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aefe6-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
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
