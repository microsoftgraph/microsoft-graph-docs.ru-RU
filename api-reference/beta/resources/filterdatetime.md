---
title: Тип ресурса FilterDatetime
description: Представляет способ фильтрации даты при фильтрации по значениям.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 27dafb0583380af299a4f5d8632c60a7e8af1a54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973557"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="8f438-103">Тип ресурса FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="8f438-103">FilterDatetime resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f438-104">Представляет способ фильтрации даты при фильтрации по значениям.</span><span class="sxs-lookup"><span data-stu-id="8f438-104">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="8f438-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f438-105">Properties</span></span>
| <span data-ttu-id="8f438-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f438-106">Property</span></span>     | <span data-ttu-id="8f438-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8f438-107">Type</span></span>   |<span data-ttu-id="8f438-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8f438-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f438-109">дата</span><span class="sxs-lookup"><span data-stu-id="8f438-109">date</span></span>|<span data-ttu-id="8f438-110">строка</span><span class="sxs-lookup"><span data-stu-id="8f438-110">string</span></span>|<span data-ttu-id="8f438-111">Дата в формате ISO8601, используемая для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="8f438-111">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="8f438-112">specificity</span><span class="sxs-lookup"><span data-stu-id="8f438-112">specificity</span></span>|<span data-ttu-id="8f438-113">string</span><span class="sxs-lookup"><span data-stu-id="8f438-113">string</span></span>|<span data-ttu-id="8f438-p101">Точность, с которой производится фильтрация данных на основе даты. Например, если указана дата 2005-04-02, а для свойства specificity задано значение month, после фильтрации останутся все строки, датированные апрелем 2009 г. Возможные значения: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="8f438-p101">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f438-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="8f438-117">Relationships</span></span>
<span data-ttu-id="8f438-118">Нет</span><span class="sxs-lookup"><span data-stu-id="8f438-118">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f438-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f438-119">JSON representation</span></span>

<span data-ttu-id="8f438-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f438-120">Here is a JSON representation of the resource.</span></span>

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
