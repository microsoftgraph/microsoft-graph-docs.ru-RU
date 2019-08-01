---
title: Тип ресурса FilterDatetime
description: Представляет способ фильтрации даты при фильтрации по значениям.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e2938c151e052372df1b959e6e24d4a2c0d94ea4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032461"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="f8fa9-103">Тип ресурса FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="f8fa9-103">FilterDatetime resource type</span></span>

<span data-ttu-id="f8fa9-104">Представляет способ фильтрации даты при фильтрации по значениям.</span><span class="sxs-lookup"><span data-stu-id="f8fa9-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="f8fa9-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8fa9-105">Properties</span></span>
| <span data-ttu-id="f8fa9-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8fa9-106">Property</span></span>     | <span data-ttu-id="f8fa9-107">Тип</span><span class="sxs-lookup"><span data-stu-id="f8fa9-107">Type</span></span>   |<span data-ttu-id="f8fa9-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f8fa9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8fa9-109">дата</span><span class="sxs-lookup"><span data-stu-id="f8fa9-109">date</span></span>|<span data-ttu-id="f8fa9-110">строка</span><span class="sxs-lookup"><span data-stu-id="f8fa9-110">string</span></span>|<span data-ttu-id="f8fa9-111">Дата в формате ISO8601, используемая для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="f8fa9-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="f8fa9-112">specificity</span><span class="sxs-lookup"><span data-stu-id="f8fa9-112">specificity</span></span>|<span data-ttu-id="f8fa9-113">string</span><span class="sxs-lookup"><span data-stu-id="f8fa9-113">string</span></span>|<span data-ttu-id="f8fa9-114">Точность, с которой производится фильтрация данных на основе даты.</span><span class="sxs-lookup"><span data-stu-id="f8fa9-114">How specific the date should be used to keep data.</span></span> <span data-ttu-id="f8fa9-115">Например, если указана дата 2005-04-02, а для свойства specificity задано значение month, после фильтрации останутся все строки, датированные апрелем 2009 г.</span><span class="sxs-lookup"><span data-stu-id="f8fa9-115">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="f8fa9-116">Допустимые значения: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="f8fa9-116">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8fa9-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="f8fa9-117">Relationships</span></span>
<span data-ttu-id="f8fa9-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f8fa9-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f8fa9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8fa9-119">JSON representation</span></span>

<span data-ttu-id="f8fa9-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8fa9-120">Here is a JSON representation of the resource.</span></span>

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
