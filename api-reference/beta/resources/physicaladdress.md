---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: eb7bf1ee21a40517704f20176f5fbcf9ea2b276a
ms.sourcegitcommit: 539ed08adf3b7ad3253c98636d4ab303ce00176e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2019
ms.locfileid: "30056989"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="74f97-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="74f97-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74f97-104">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="74f97-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="74f97-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="74f97-105">Properties</span></span>
| <span data-ttu-id="74f97-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="74f97-106">Property</span></span>     | <span data-ttu-id="74f97-107">Тип</span><span class="sxs-lookup"><span data-stu-id="74f97-107">Type</span></span>   |<span data-ttu-id="74f97-108">Описание</span><span class="sxs-lookup"><span data-stu-id="74f97-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74f97-109">city</span><span class="sxs-lookup"><span data-stu-id="74f97-109">city</span></span>|<span data-ttu-id="74f97-110">String</span><span class="sxs-lookup"><span data-stu-id="74f97-110">String</span></span>|<span data-ttu-id="74f97-111">Город.</span><span class="sxs-lookup"><span data-stu-id="74f97-111">The city.</span></span>|
|<span data-ttu-id="74f97-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="74f97-112">countryOrRegion</span></span>|<span data-ttu-id="74f97-113">String</span><span class="sxs-lookup"><span data-stu-id="74f97-113">String</span></span>|<span data-ttu-id="74f97-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="74f97-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="74f97-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="74f97-116">postalCode</span></span>|<span data-ttu-id="74f97-117">String</span><span class="sxs-lookup"><span data-stu-id="74f97-117">String</span></span>|<span data-ttu-id="74f97-118">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="74f97-118">The postal code.</span></span>|
|<span data-ttu-id="74f97-119">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="74f97-119">postOfficeBox</span></span>|<span data-ttu-id="74f97-120">String</span><span class="sxs-lookup"><span data-stu-id="74f97-120">String</span></span>|<span data-ttu-id="74f97-121">Номер почтового ящика в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="74f97-121">The post office box number.</span></span>|
|<span data-ttu-id="74f97-122">state</span><span class="sxs-lookup"><span data-stu-id="74f97-122">state</span></span>|<span data-ttu-id="74f97-123">String</span><span class="sxs-lookup"><span data-stu-id="74f97-123">String</span></span>|<span data-ttu-id="74f97-124">Штат.</span><span class="sxs-lookup"><span data-stu-id="74f97-124">The state.</span></span>|
|<span data-ttu-id="74f97-125">street</span><span class="sxs-lookup"><span data-stu-id="74f97-125">street</span></span>|<span data-ttu-id="74f97-126">String</span><span class="sxs-lookup"><span data-stu-id="74f97-126">String</span></span>|<span data-ttu-id="74f97-127">Улица.</span><span class="sxs-lookup"><span data-stu-id="74f97-127">The street.</span></span>|
|<span data-ttu-id="74f97-128">type</span><span class="sxs-lookup"><span data-stu-id="74f97-128">type</span></span>|<span data-ttu-id="74f97-129">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="74f97-129">physicalAddressType</span></span>|<span data-ttu-id="74f97-130">Тип адреса.</span><span class="sxs-lookup"><span data-stu-id="74f97-130">The type of address.</span></span> <span data-ttu-id="74f97-131">Возможные значения: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="74f97-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="74f97-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74f97-132">JSON representation</span></span>

<span data-ttu-id="74f97-133">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="74f97-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "postalCode": "string",
  "postOfficeBox": "string",
  "state": "string",
  "street": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/physicaladdress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}-->
