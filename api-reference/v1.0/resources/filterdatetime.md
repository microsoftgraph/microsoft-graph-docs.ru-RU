---
title: Тип ресурса FilterDatetime
description: Представляет способ фильтрации даты при фильтрации по значениям.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bd8d7c01b94306245708df8290a44ffb936ac4d6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018293"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="0d72d-103">Тип ресурса FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="0d72d-103">FilterDatetime resource type</span></span>

<span data-ttu-id="0d72d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d72d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d72d-105">Представляет способ фильтрации даты при фильтрации по значениям.</span><span class="sxs-lookup"><span data-stu-id="0d72d-105">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="0d72d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d72d-106">Properties</span></span>
| <span data-ttu-id="0d72d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d72d-107">Property</span></span>     | <span data-ttu-id="0d72d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0d72d-108">Type</span></span>   |<span data-ttu-id="0d72d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0d72d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d72d-110">дата</span><span class="sxs-lookup"><span data-stu-id="0d72d-110">date</span></span>|<span data-ttu-id="0d72d-111">string</span><span class="sxs-lookup"><span data-stu-id="0d72d-111">string</span></span>|<span data-ttu-id="0d72d-112">Дата в формате ISO8601, используемая для фильтрации данных.</span><span class="sxs-lookup"><span data-stu-id="0d72d-112">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="0d72d-113">specificity</span><span class="sxs-lookup"><span data-stu-id="0d72d-113">specificity</span></span>|<span data-ttu-id="0d72d-114">string</span><span class="sxs-lookup"><span data-stu-id="0d72d-114">string</span></span>|<span data-ttu-id="0d72d-115">Точность, с которой производится фильтрация данных на основе даты.</span><span class="sxs-lookup"><span data-stu-id="0d72d-115">How specific the date should be used to keep data.</span></span> <span data-ttu-id="0d72d-116">Например, если указана дата 2005-04-02, а для свойства specificity задано значение month, после фильтрации останутся все строки, датированные апрелем 2009 г.</span><span class="sxs-lookup"><span data-stu-id="0d72d-116">For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009.</span></span> <span data-ttu-id="0d72d-117">Допустимые значения: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span><span class="sxs-lookup"><span data-stu-id="0d72d-117">The possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d72d-118">Связи</span><span class="sxs-lookup"><span data-stu-id="0d72d-118">Relationships</span></span>
<span data-ttu-id="0d72d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0d72d-119">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0d72d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d72d-120">JSON representation</span></span>

<span data-ttu-id="0d72d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d72d-121">Here is a JSON representation of the resource.</span></span>

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

