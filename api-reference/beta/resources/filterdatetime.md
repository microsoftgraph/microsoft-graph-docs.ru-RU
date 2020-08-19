---
title: Тип ресурса FilterDatetime
description: Представляет способ фильтрации даты при фильтрации по значениям.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ruoyingl
ms.openlocfilehash: 71d0f3dc82882b0726d98c2b7fd2b60bb215152a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809821"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="7519f-103">Тип ресурса FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="7519f-103">FilterDatetime resource type</span></span>

<span data-ttu-id="7519f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7519f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7519f-105">Представляет способ фильтрации даты при фильтрации по значениям.</span><span class="sxs-lookup"><span data-stu-id="7519f-105">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="7519f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7519f-106">Properties</span></span>
| <span data-ttu-id="7519f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7519f-107">Property</span></span>     | <span data-ttu-id="7519f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7519f-108">Type</span></span>   |<span data-ttu-id="7519f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7519f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7519f-110">дата</span><span class="sxs-lookup"><span data-stu-id="7519f-110">date</span></span>|<span data-ttu-id="7519f-111">string</span><span class="sxs-lookup"><span data-stu-id="7519f-111">string</span></span>|<span data-ttu-id="7519f-112">Дата в формате ISO8601, используемая для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="7519f-112">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="7519f-113">specificity</span><span class="sxs-lookup"><span data-stu-id="7519f-113">specificity</span></span>|<span data-ttu-id="7519f-114">string</span><span class="sxs-lookup"><span data-stu-id="7519f-114">string</span></span>|<span data-ttu-id="7519f-p101">Точность, с которой производится фильтрация данных на основе даты. Например, если указана дата 2005-04-02, а для свойства specificity задано значение month, после фильтрации останутся все строки, датированные апрелем 2009 г. Возможные значения: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="7519f-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7519f-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="7519f-118">Relationships</span></span>
<span data-ttu-id="7519f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="7519f-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7519f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7519f-120">JSON representation</span></span>

<span data-ttu-id="7519f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7519f-121">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
