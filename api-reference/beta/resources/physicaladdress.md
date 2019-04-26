---
title: Тип ресурса physicalAddress
description: Представляет почтовый адрес ресурса, например контакта или события.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: d6081f21069cef6014c8a028898f11ea9a3f4f3c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345010"
---
# <a name="physicaladdress-resource-type"></a><span data-ttu-id="b86f1-103">Тип ресурса physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b86f1-103">physicalAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b86f1-104">Представляет почтовый адрес ресурса, например контакта или события.</span><span class="sxs-lookup"><span data-stu-id="b86f1-104">Represents the street address of a resource such as a contact or event.</span></span>


## <a name="properties"></a><span data-ttu-id="b86f1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b86f1-105">Properties</span></span>
| <span data-ttu-id="b86f1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b86f1-106">Property</span></span>     | <span data-ttu-id="b86f1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b86f1-107">Type</span></span>   |<span data-ttu-id="b86f1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b86f1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b86f1-109">city</span><span class="sxs-lookup"><span data-stu-id="b86f1-109">city</span></span>|<span data-ttu-id="b86f1-110">String</span><span class="sxs-lookup"><span data-stu-id="b86f1-110">String</span></span>|<span data-ttu-id="b86f1-111">Город.</span><span class="sxs-lookup"><span data-stu-id="b86f1-111">The city.</span></span>|
|<span data-ttu-id="b86f1-112">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="b86f1-112">countryOrRegion</span></span>|<span data-ttu-id="b86f1-113">String</span><span class="sxs-lookup"><span data-stu-id="b86f1-113">String</span></span>|<span data-ttu-id="b86f1-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="b86f1-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="b86f1-116">postalCode</span><span class="sxs-lookup"><span data-stu-id="b86f1-116">postalCode</span></span>|<span data-ttu-id="b86f1-117">String</span><span class="sxs-lookup"><span data-stu-id="b86f1-117">String</span></span>|<span data-ttu-id="b86f1-118">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="b86f1-118">The postal code.</span></span>|
|<span data-ttu-id="b86f1-119">postOfficeBox</span><span class="sxs-lookup"><span data-stu-id="b86f1-119">postOfficeBox</span></span>|<span data-ttu-id="b86f1-120">String</span><span class="sxs-lookup"><span data-stu-id="b86f1-120">String</span></span>|<span data-ttu-id="b86f1-121">Номер почтового ящика в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b86f1-121">The post office box number.</span></span>|
|<span data-ttu-id="b86f1-122">state</span><span class="sxs-lookup"><span data-stu-id="b86f1-122">state</span></span>|<span data-ttu-id="b86f1-123">String</span><span class="sxs-lookup"><span data-stu-id="b86f1-123">String</span></span>|<span data-ttu-id="b86f1-124">Штат.</span><span class="sxs-lookup"><span data-stu-id="b86f1-124">The state.</span></span>|
|<span data-ttu-id="b86f1-125">street</span><span class="sxs-lookup"><span data-stu-id="b86f1-125">street</span></span>|<span data-ttu-id="b86f1-126">String</span><span class="sxs-lookup"><span data-stu-id="b86f1-126">String</span></span>|<span data-ttu-id="b86f1-127">Улица.</span><span class="sxs-lookup"><span data-stu-id="b86f1-127">The street.</span></span>|
|<span data-ttu-id="b86f1-128">type</span><span class="sxs-lookup"><span data-stu-id="b86f1-128">type</span></span>|<span data-ttu-id="b86f1-129">physicalAddressType</span><span class="sxs-lookup"><span data-stu-id="b86f1-129">physicalAddressType</span></span>|<span data-ttu-id="b86f1-130">Тип адреса.</span><span class="sxs-lookup"><span data-stu-id="b86f1-130">The type of address.</span></span> <span data-ttu-id="b86f1-131">Возможные значения: `unknown`, `home`, `business`, `other`.</span><span class="sxs-lookup"><span data-stu-id="b86f1-131">Possible values are: `unknown`, `home`, `business`, `other`.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b86f1-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b86f1-132">JSON representation</span></span>

<span data-ttu-id="b86f1-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b86f1-133">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "physicalAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
