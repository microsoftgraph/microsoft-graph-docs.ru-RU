---
title: Тип ресурса Посталаддресс
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7d168e4f53dbd182e4dbd93d0a5b6342daf3339d
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30057413"
---
# <a name="postaladdress-resource-type"></a><span data-ttu-id="14504-103">Тип ресурса Посталаддресс</span><span class="sxs-lookup"><span data-stu-id="14504-103">postalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14504-104">Представляет почтовый адрес расположения.</span><span class="sxs-lookup"><span data-stu-id="14504-104">Represents the street address of a location.</span></span>


## <a name="properties"></a><span data-ttu-id="14504-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="14504-105">Properties</span></span>
| <span data-ttu-id="14504-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="14504-106">Property</span></span>     | <span data-ttu-id="14504-107">Тип</span><span class="sxs-lookup"><span data-stu-id="14504-107">Type</span></span>   |<span data-ttu-id="14504-108">Описание</span><span class="sxs-lookup"><span data-stu-id="14504-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14504-109">city</span><span class="sxs-lookup"><span data-stu-id="14504-109">city</span></span>|<span data-ttu-id="14504-110">String</span><span class="sxs-lookup"><span data-stu-id="14504-110">String</span></span>|<span data-ttu-id="14504-111">Город.</span><span class="sxs-lookup"><span data-stu-id="14504-111">The city.</span></span>|
|<span data-ttu-id="14504-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="14504-112">countryOrRegion</span></span>|<span data-ttu-id="14504-113">String</span><span class="sxs-lookup"><span data-stu-id="14504-113">String</span></span>|<span data-ttu-id="14504-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="14504-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="14504-116">Исинферред</span><span class="sxs-lookup"><span data-stu-id="14504-116">isInferred</span></span>|<span data-ttu-id="14504-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="14504-117">Boolean</span></span>|<span data-ttu-id="14504-118">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="14504-118">For internal use only.</span></span>|
|<span data-ttu-id="14504-119">postalCode</span><span class="sxs-lookup"><span data-stu-id="14504-119">postalCode</span></span>|<span data-ttu-id="14504-120">String</span><span class="sxs-lookup"><span data-stu-id="14504-120">String</span></span>|<span data-ttu-id="14504-121">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="14504-121">The postal code.</span></span>|
|<span data-ttu-id="14504-122">state</span><span class="sxs-lookup"><span data-stu-id="14504-122">state</span></span>|<span data-ttu-id="14504-123">String</span><span class="sxs-lookup"><span data-stu-id="14504-123">String</span></span>|<span data-ttu-id="14504-124">Штат.</span><span class="sxs-lookup"><span data-stu-id="14504-124">The state.</span></span>|
|<span data-ttu-id="14504-125">street</span><span class="sxs-lookup"><span data-stu-id="14504-125">street</span></span>|<span data-ttu-id="14504-126">String</span><span class="sxs-lookup"><span data-stu-id="14504-126">String</span></span>|<span data-ttu-id="14504-127">Улица.</span><span class="sxs-lookup"><span data-stu-id="14504-127">The street.</span></span>|
|<span data-ttu-id="14504-128">type</span><span class="sxs-lookup"><span data-stu-id="14504-128">type</span></span>|<span data-ttu-id="14504-129">addressType</span><span class="sxs-lookup"><span data-stu-id="14504-129">addressType</span></span>|<span data-ttu-id="14504-130">Тип адреса.</span><span class="sxs-lookup"><span data-stu-id="14504-130">The type of address.</span></span> <span data-ttu-id="14504-131">`unknown`Возможные значения: `home`,, `business`,. `other`</span><span class="sxs-lookup"><span data-stu-id="14504-131">The possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="14504-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14504-132">JSON representation</span></span>

<span data-ttu-id="14504-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14504-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.postalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "isInferred": "boolean",
  "postalCode": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "postaladdress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/postaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
