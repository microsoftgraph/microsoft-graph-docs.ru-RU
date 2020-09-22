---
title: Тип ресурса Фисикалоффицеаддресс
description: Представляет рабочий адрес ресурса, например контакт или событие.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a3c1bee1c8617fbe93ad28f821b1042901065400
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088477"
---
# <a name="physicalofficeaddress-resource-type"></a><span data-ttu-id="41dbd-103">Тип ресурса Фисикалоффицеаддресс</span><span class="sxs-lookup"><span data-stu-id="41dbd-103">physicalOfficeAddress resource type</span></span>

<span data-ttu-id="41dbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41dbd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41dbd-105">Представляет рабочий адрес ресурса, например контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="41dbd-105">Represents the business address of a resource such as an organizational contact.</span></span>

## <a name="properties"></a><span data-ttu-id="41dbd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="41dbd-106">Properties</span></span>

| <span data-ttu-id="41dbd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="41dbd-107">Property</span></span>     | <span data-ttu-id="41dbd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="41dbd-108">Type</span></span>   |<span data-ttu-id="41dbd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="41dbd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41dbd-110">city</span><span class="sxs-lookup"><span data-stu-id="41dbd-110">city</span></span>|<span data-ttu-id="41dbd-111">String</span><span class="sxs-lookup"><span data-stu-id="41dbd-111">String</span></span>|<span data-ttu-id="41dbd-112">Город.</span><span class="sxs-lookup"><span data-stu-id="41dbd-112">The city.</span></span>|
|<span data-ttu-id="41dbd-113">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="41dbd-113">countryOrRegion</span></span>|<span data-ttu-id="41dbd-114">String</span><span class="sxs-lookup"><span data-stu-id="41dbd-114">String</span></span>|<span data-ttu-id="41dbd-p101">Страна или регион. Это строковое значение в произвольном формате, например "США".</span><span class="sxs-lookup"><span data-stu-id="41dbd-p101">The country or region. It's a free-format string value, for example, "United States".</span></span>|
|<span data-ttu-id="41dbd-117">officeLocation</span><span class="sxs-lookup"><span data-stu-id="41dbd-117">officeLocation</span></span>  | <span data-ttu-id="41dbd-118">String</span><span class="sxs-lookup"><span data-stu-id="41dbd-118">String</span></span> | <span data-ttu-id="41dbd-119">Местоположение Office, например здание и номер офиса для контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="41dbd-119">Office location such as building and office number for an organizational contact.</span></span>  |
|<span data-ttu-id="41dbd-120">postalCode</span><span class="sxs-lookup"><span data-stu-id="41dbd-120">postalCode</span></span>|<span data-ttu-id="41dbd-121">String</span><span class="sxs-lookup"><span data-stu-id="41dbd-121">String</span></span>|<span data-ttu-id="41dbd-122">Почтовый индекс.</span><span class="sxs-lookup"><span data-stu-id="41dbd-122">The postal code.</span></span>|
|<span data-ttu-id="41dbd-123">state</span><span class="sxs-lookup"><span data-stu-id="41dbd-123">state</span></span>|<span data-ttu-id="41dbd-124">String</span><span class="sxs-lookup"><span data-stu-id="41dbd-124">String</span></span>|<span data-ttu-id="41dbd-125">Штат.</span><span class="sxs-lookup"><span data-stu-id="41dbd-125">The state.</span></span>|
|<span data-ttu-id="41dbd-126">street</span><span class="sxs-lookup"><span data-stu-id="41dbd-126">street</span></span>|<span data-ttu-id="41dbd-127">String</span><span class="sxs-lookup"><span data-stu-id="41dbd-127">String</span></span>|<span data-ttu-id="41dbd-128">Улица.</span><span class="sxs-lookup"><span data-stu-id="41dbd-128">The street.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41dbd-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41dbd-129">JSON representation</span></span>

<span data-ttu-id="41dbd-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41dbd-130">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

